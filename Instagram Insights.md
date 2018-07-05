# Instagram Insights

Selection of metrics from instagram insights organized by categories.

## User Insights
Getting Account Insights

To get insights for an Instagram Business Account, send a GET request to the /user/insights edge and include the metric parameter with one or more metrics, as well as the period parameter and a timeframe (e.g. daily impressions or weekly impressions).

```
GET graph.facebook.com
  /17841405822304914/insights?metric=impressions,reach,profile_views&period=day
```

### Permissions
A User access token with the following permissions:

- instagram_basics
- instagram_manage_insights
- manage_pages

##### audience_city
The cities of the Business Account's followers. Does not include current day's data.
*lifetime*
##### audience_country
The countries of the Business Account's followers. Does not include current day's data.
*lifetime*
##### audience_gender_age
The gender and age distribution of the Business Account's followers. Does not include current day's data.
*lifetime*
##### audience_locale
The locales by country codes of the Business Account's followers. Does not include current day's data.
*lifetime*
##### email_contacts
Total number of taps on the email link in the Business Account's profile.
*day*
##### follower_count
Total number of unique users following the Business Account.
*day*
##### get_directions_clicks
Total number of taps on the directions link in the Business Account's profile.
*day*
##### impressions
Total number of times the Business Account's media objects (i.e. posts, stories and promotions) have been viewed. Does not include profile views.
*day, week, days_28*
##### online_followers
Total number of the Business Account's followers who were online during the specified period.
*lifetime*
##### phone_call_clicks
Total number of taps on the call link in the Business Account's profile.
*day*
##### profile_views
Total number of unique users who have viewed the Business Account's profile within the specified period.
*day*
##### reach
Total number of unique users who have viewed the Business Account's profile.
*day, week, days_28*
##### text_message_clicks
Total number of taps on the text message link in the Business Account's profile.
*day*
##### website_clicks
Total number of taps on the website link in the Business Account's profile.
*day*

## Media Insights
To get insights data for an individual media object, send a GET request to the /media/insights edge and include the metric parameter with one or more of the metric values you want returned. Please note the following limitations:

- Insights data is not available for media objects within album carousels (children).
- Stories insights are only available for 24 hours, even if the stories are archived or highlighted. If you want to get the latest insights for a story before it expires, set up a Webhook for the Instagram topic and subscribe to the story_insights field.

````
GET graph.facebook.com
  /17895695668004550/insights?metric=impressions,reach
````

### Photo & Video Metrics

##### engagement
likes, comments, and saves
##### impressions

##### reach

##### saved

##### video_views
videos only

## Carousel Album Metrics

##### carousel_album_engagement

##### carousel_album_impressions

##### carousel_album_reach

##### carousel_album_saved

##### carousel_album_video_views