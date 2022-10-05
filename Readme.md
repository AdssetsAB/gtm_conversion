# ACM Site Tracking GTM

Template designed for Adssets/ACM ad server in order to gather conversion and custom tracking, allowing extra flexibility to the service.

## How to use

1 - Set up the template in your GTM account
2 - Create a new tag and select the template
3 - Fill the fields with the information provided by your Adssets/ACM account manager (AdvertiserId can be found in the URL of ACM when listing the campaigns for a given advertiser).
4 - Save the tag and publish the container.

## Parameter description

- AdvertiserId: The ID of the advertiser in ACM
- Send Event: The name of the event to be sent when this tag is triggered and there is an incomming request from a campaign with conversions enabled.
- ProductId: The ID of the product in the FEED uploaded in ACM for the campaign. If null no product information will be sent.
- Product viewed or bought: If the product id is set the tag can specify if the event should trigger the bought or the viewed pixel for this tag to be used for retargeting propouses.
- DSP Retargeting: Allows the user to specify if the tag should trigger the pixel of the specified DSP for retargeting propouses or should not use any id.

## Consents

- ad_storage : If the user has given consent to store information about the user or his/her device for the purpose of serving targeted ads.
- ad_personalization: If the user has given consent to the collection and processing of information about the user or his/her device for the purpose of serving targeted ads.

Retargeting tags with ids will only be sent if ad_personalization is set.
No cookies will be saved if ad_storage is not set preventing some of the tracking to work after landing into the page.



