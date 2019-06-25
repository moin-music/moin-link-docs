# Facebook Pixel

## Facebook Pixel Support

With the Facebook Pixel integration you can create Custom Audiences that can be used to target your Facebook Ads based on the visitors of your [moin.link](https://moin.link) landing page.

An audience can be defined as a simple `All website visitors`, a more refined `Every visitor who clicked on Spotify or Deezer` or even a `Every visitor without any link click` \(aka bouncer\).

Here's a step-by-step guide explaining the process end-to-end

## 1. Setup

### 1.1 Create Facebook Pixel

1. Log into the [Facebook Business Manager](https://business.facebook.com)
2. Click on the `≡ Business Manager` button
3. Click on `All tools`
4. Click on  `Measure & report > Events Manager > Pixels`

![](.gitbook/assets/screenshot-2019-06-25-at-10.08.42%20%281%29.png)

1. Click on `+ Add New Data Source`
2. Click on `Facebook pixel`

![](.gitbook/assets/screenshot-2019-06-25-at-10.12.09%20%281%29.png)

1. Pick a name and leave the `Website URL` empty
2. Hit `Create`

> ![Screenshot 2019-06-21 at 11.11.57.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/6fbcec6c.png%20=500x)

### 1.2 Copy Pixel Code

Select `Manually install pixel code yourself`:

> ![Screenshot 2019-06-21 at 11.09.37.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/f5424f1d.png%20=400x)

Click on the code to copy it:

> ![Screenshot 2019-06-21 at 11.09.22.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/a8731e48.png%20=500x)

### 1.3 Integrate Facebook Pixel

1. Log into your [moin.link](https://moin.link) page and open the menu by hovering over the moin.link logo in top left corner
2. Click on `Tracking Pixels`
3. Click on `Facebook`
4. Paste the Pixel Code into the Textbox
5. Hit `Add`

> ![Screenshot 2019-06-20 at 15.36.41.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/89093796.png%20=400x)

Now your pixel is installed!

### 1.4 Choose Your Cookie Consent

The Facebook Pixel can only be served to visitors who have given their explicit consent. By default this consent is shown.

#### 1.4.1 Default

> ![Screenshot 2019-06-21 at 15.59.23.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/43f0706d.png%20=400x)

Once the visitor hits accept, the Facebook Pixel is served and this user can be part of a Custom Audience.

#### 1.4.2 Force Visitor Decision

Alternatively

> ![Screenshot 2019-06-21 at 16.01.30.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/8c52544e.png%20=400x)

## 2. Retargeting \(aka Remarketing\)

The pixel triggers different events for different visitor actions. You can create audiences based on those events. To create an audience go to the [Facebook Business Manager](https://business.facebook.com) and navigate to `Menu > All tools > Assets > Audiences`:

> ![Screenshot 2019-06-21 at 12.34.48.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/4373007b.png%20=600x)

1. Click on `Create Audience`
2. Click on `Custom Audience`

> ![Screenshot 2019-06-21 at 12.39.36.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/df264247.png%20=500x)

Choose `Website traffic`:

> ![Screenshot 2019-06-21 at 12.50.52.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/a7d39764.png%20=400x)

Now you have different options depending on what kind of visitors you want to target:

### 2.1 All Visitors

The most basic audience targets every visitor of your moin.link page:

1. Select your pixel
2. Pick `All website visitors`
3. Name your audience
4. Hit `Create Audience`

> ![Screenshot 2019-06-21 at 12.50.28.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/55bd62e1.png%20=600x)

### 2.2 Visitors who have clicked a certain link

You can also target visitors who have clicked on a certain link, e.g. Spotify

> Please wait a few days after integrating your pixel. Otherwise Facebook won't know about the different possible events from your landing page and you won't be able to select them.

1. Pick `Outlink` \(instead of `All website visitors`\)
2. Click on `Refine by`
3. Choose `URL/Parameter`
4. Select `label`
5. Choose a service name, e.g. `spotify`
6. Name your audience
7. Hit `Create Audience`

> ![Screenshot 2019-06-21 at 13.21.58.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/7cb10f1d.png%20=300x)
>
> ![Screenshot 2019-06-21 at 13.18.25.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/d0726724.png%20=600x)

### 2.3 Visitors without any link clicks aka bouncers

It is also possible to target everyone who hasn't clicked on any link. This is an important audience as in todays busy life we tend to get distracted and forget to finish an intention. Now you can reengage with those visitors too!

Just choose `Bounce` as the pixel criteria \(instead of `All website visitors`\):

> ![Screenshot 2019-06-21 at 13.25.58.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/1cf4fd84.png%20=300x)

## 3. Possible filter criteria

The parameter action contains the type of link the visitor clicked on, possible values are:

* Stream
* Download
* Vinyl
* Live
* Artist

The parameter label contains the actual link target, possible values are:

* spotify
* itunes
* bandcamp
* ...

and many more! Here's a way how you can figure out the right parameters yourself:

In the [Facebook Business Manager](https://business.facebook.com) select your pixel on the `Measure & report > Events Manager > Pixels` page:

> ![Screenshot 2019-06-21 at 13.57.25.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/da25ac74.png%20=700x)

Here you see all the possible actions \(PageView, Outlink, Bounce\) that have already happend on your landing page. To learn more about possible labels, click on `View details`:

> ![Screenshot 2019-06-21 at 14.03.10.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/48bdb0b5.png%20=700x)

Select the `Activity` tab and hover the `Parameters` column to see more details:

> ![Screenshot 2019-06-21 at 14.07.28.png](:storage/9d15ddac-a0b1-4eea-8ef2-08376f997a4c/c0c1faf2.png%20=600x)

If you think some label is missing here, just click the corresponding link on your landing page by yourself and it will appear here shortly.

