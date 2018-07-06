# Facebook Insights

Selection of metrics from facebook insights organized by categories.

### Permissions
A Page access token with read_insights permissions

### Naming Patterns for Metrics
The _unique suffix indicates that this metric shows the number of unique users who performed a specific action. Metrics generated with the _unique suffix are approximate and may not be 100% accurate.

The _login and _logout suffixes indicate whether someone was logged into or out of Facebook.

The _source suffix indicates that the metric will be broken down into a list of referral sources. External referrals are broken down by domain. Internal referrals are broken down by Facebook-specific features such as 'Profile', 'Search', 'Requests', 'Suggestions', 'Stream', etc. In these case the value returned will be an object containing a series of key-value pairs where the key is the source name and the value is the metric for that source.

Most metrics will update once every 24 hours. Some metrics, marked with an *, are refreshed several times during the day.

## Global Stats
### Page and Post Stories and "People talking about this"
#### Time framed stats
##### page_content_activity
The number of stories created about your Page (Stories).
*day, week, days_28*
##### page_content_activity_by_action_type
The number of stories about your Page's stories, by Page story type.
*day, week, days_28*
##### page_content_activity_by_action_type_unique	
The number of people talking about your Page's stories, by Page story type.
*day, week, days_28*
##### page_content_activity_by_age_gender_unique
The number of People Talking About the Page by user age and gender.
*day, week, days_28*
##### page_content_activity_by_country_unique
The number of people, aggregated per country, that are talking about your Page. Only the 45 countries with the most people talking about your page are included.
*day, week, days_28*
##### page_content_activity_by_city_unique
The number of People Talking About the Page by user city.
*day, week, days_28*
##### page_content_activity_by_locale_unique
The number of People Talking About the Page by user language.
*day, week, days_28*
#### Lifetime Stats
##### post_activity*	
The number of stories generated about your Page post ('Stories').
*lifetime*
##### post_activity_unique*
The number of unique people who created a story about your Page post ('People Talking About This' / PTAT).
*lifetime*
##### post_activity_by_action_type*	
The number of stories created about your Page post, by action type.
*lifetime*
##### post_activity_by_action_type_unique*	
The number of unique people who created a story about your Page post, by action type.
*lifetime*

### Page Impressions
Note that the unique impression insights values are calculated independently. Total page reach may not always be exactly equal to the sum of viral_unique and organic_unique.
##### page_impressions*
The number of times any content from your Page or about your Page entered a person's screen. This includes posts, check-ins, ads, social information from people who interact with your Page and more.
*day, week, days_28*
##### page_impressions_unique*
The number of people who had any content from your Page or about your Page enter their screen. This includes posts, check-ins, ads, social information from people who interact with your Page and more.
*day, week, days_28*
##### page_impressions_paid*
The number of times any content from your Page or about your Page entered a person's screen through paid distribution such as an ad.
*day, week, days_28*
##### page_impressions_paid_unique*	
The number of people who had any content from your Page or about your Page enter their screen through paid distribution such as an ad.
*day, week, days_28*
##### page_impressions_organic*
The number of times any content from your Page or about your Page entered a person's screen through unpaid distribution. This includes posts, check-ins, social information from people who interact with your Page and more.
*day, week, days_28*
##### page_impressions_organic_unique*	
The number of people who had any content from your Page or about your Page enter their screen through unpaid distribution. This includes posts, check-ins, social information from people who interact with your Page and more.
*day, week, days_28*
##### page_impressions_viral*
The number of times any content from your Page or about your Page entered a person's screen with social information attached. Social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_impressions_viral_unique*	
The number of people who had any content from your Page or about your Page enter their screen through with social information attached. As a form of organic distribution, social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_impressions_nonviral*	
The number of times any content from your Page entered a person's screen. This does not include content created about your Page with social information attached. Social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_impressions_nonviral_unique*	
The number of people who had any content from your Page enter their screen. This does not include content created about your Page with social information attached. As a form of organic distribution, social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_impressions_by_story_type	
Total impressions of stories published by a friend about your Page by story type.
*day, week, days_28*

| Name | Description
| ------ | ------
| checkin | Page checkins
| coupon | Offer claims
| event | RSVPing to event
| fan | Page likes
| mention | Page mentions
| page post | Posts by a Page
| question | Question answers
| user post | Posts by people on a Page
| other | Other types
##### page_impressions_by_story_type_unique	
The number of people who saw stories published by a friend about your Page by story type.
*day, week, days_28*

| Name | Description
| ------ | ------
| checkin | Page checkins
| coupon | Offer claims
| event | RSVPing to event
| fan | Page likes
| mention | Page mentions
| page post | Posts by a Page
| question | Question answers
| user post | Posts by people on a Page
| other | Other types
##### page_impressions_by_city_unique
The number of people who have seen any content associated with your Page by city.
*day, week, days_28*
##### page_impressions_by_country_unique
The number of people who have seen any content associated with your Page by country.
*day, week, days_28*
##### page_impressions_by_locale_unique
The number of people who have seen any content associated with your Page by user selected language.
*day, week, days_28*
##### page_impressions_by_age_gender_unique
The number of people who saw any content by your Page or about your Page, grouped by age and gender.
*day, week, days_28*
##### page_impressions_frequency_distribution
The number of people your Page reached broken down by how many times people saw any content about your Page.
*day, week, days_28*
##### page_impressions_viral_frequency_distribution
The number of people your Page reached from a story published by a friend, broken down by how many times people saw stories about your Page.
*day, week, days_28*

### Page Engagement
##### page_engaged_users
The number of people who engaged with your Page. Engagement includes any click.
*day, week, days_28*
##### page_post_engagements*
The number of times people have engaged with your posts through likes, comments and shares and more.
*day, week, days_28*
##### page_consumptions
The number of times people clicked on any of your content.
*day, week, days_28*
##### page_consumptions_unique	
The number of people who clicked on any of your content.
*day, week, days_28*
##### page_consumptions_by_consumption_type
The number of times people clicked on any of your content, by type.
*day, week, days_28*
##### page_consumptions_by_consumption_type_unique
The number of people who clicked on any of your content, by type.
*day, week, days_28*
##### page_places_checkin_total
The number of times people checked into a place.
*day, week, days_28*
##### page_places_checkin_total_unique
The number of people who checked into a place.
*day, week, days_28*
##### page_places_checkin_mobile
The number of times people checked into a place using mobile phones.
*day, week, days_28*
##### page_places_checkin_mobile_unique
The number of people who checked into a place using mobile phones.
*day, week, days_28*
##### page_places_checkins_by_age_gender
gender and age of people who checked in at your Place.
*day*
##### page_places_checkins_by_locale
top locales of people who checked into your Place.
*day*
##### page_places_checkins_by_country
top countries of people who checked into your Place.
*day*
##### page_negative_feedback
The number of times people took a negative action (e.g., un-liked or hid a post).
*day, week, days_28*
##### page_negative_feedback_unique	
The number of people who took a negative action (e.g., un-liked or hid a post).
*day, week, days_28*
##### page_negative_feedback_by_type
The number of times people took a negative action broken down by type.
*day, week, days_28*

| Name | Description
| ------ | ------
| hide_clicks | Hide this story
| hide_all_clicks | Hide all posts from this page
| report_spam_clicks | Report an object as a spam
| unlike_page_clicks | Unlike a page
| xbutton_clicks | Deprecated. This is no longer logged
##### page_negative_feedback_by_type_unique	
The number of people who took a negative action broken down by type. (See possible types)
*day, week, days_28*

| Name | Description
| ------ | ------
| hide_clicks | Hide this story
| hide_all_clicks | Hide all posts from this page
| report_spam_clicks | Report an object as a spam
| unlike_page_clicks | Unlike a page
| xbutton_clicks | Deprecated. This is no longer logged
##### page_positive_feedback_by_type
The number of times people took a positive action broken down by type
*day, week, days_28*

| Name | Description
| ------ | ------
| like | Like a story
| comment | Comment on a story
|link|Share a story
|answer	|Answer a question
|claim	|Claim an offer
|rsvp|Respond to an event
##### page_positive_feedback_by_type_unique	
The number of people who took a positive action broken down by type. (See possible types)
*day, week, days_28*

| Name | Description
| ------ | ------
| like | Like a story
| comment | Comment on a story
|link|Share a story
|answer	|Answer a question
|claim	|Claim an offer
|rsvp|Respond to an event
##### page_fans_online	
The number of your fans who saw any posts on Facebook on a given day, broken down by hour of day in PST/PDT.
*day*
##### page_fans_online_per_day
The number of your fans who saw any posts on Facebook on a given day.
*day*
##### page_fan_adds_by_paid_non_paid_unique	
The number of new people who have liked your page broken down by paid and non-paid.
*day*

### Page Reactions
##### page_actions_post_reactions_like_total
Daily total post "like" reactions of a page.
*day*
##### page_actions_post_reactions_love_total
Daily total post "love" reactions of a page.
*day*
##### page_actions_post_reactions_wow_total
Daily total post "wow" reactions of a page.
*day*
##### page_actions_post_reactions_haha_total
Daily total post "haha" reactions of a page.
*day*
##### page_actions_post_reactions_sorry_total
Daily total post "sorry" reactions of a page.
*day*
##### page_actions_post_reactions_anger_total
Daily total post "anger" reactions of a page.
*day*
##### page_actions_post_reactions_total	
Daily total post reactions of a page by type.
*day*

### Page CTA Clicks
##### page_total_actions
The number of clicks on your Page's contact info and call-to-action button.
*day, week, days_28*
##### page_cta_clicks_logged_in_total
Total number of clicks on the Page CTA button by people who are logged in to Facebook.
*day, week, days_28*
##### page_cta_clicks_logged_in_unique
Unique number of clicks on the Page CTA button by people who are logged in to Facebook.
*day, week, days_28*
##### page_cta_clicks_by_site_logged_in_unique
Number of unique people who are logged in to Facebook and clicked on the CTA button, broken down by www, mobile, api or other.
*day, week, days_28*
##### page_cta_clicks_by_age_gender_logged_in_unique
Number of unique people who are logged in to Facebook and clicked the Page CTA button, broken down by age and gender group.
*day, week, days_28*
##### page_cta_clicks_logged_in_by_country_unique
Number of unique people who are logged in to Facebook and clicked the Page CTA button, broken down by country.
*day, week, days_28*
##### page_cta_clicks_logged_in_by_city_unique
Number of unique people who are logged in to Facebook and clicked the Page CTA button, broken down by city.
*day, week, days_28*
##### page_call_phone_clicks_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Call Now button.
*day, week, days_28*
##### page_call_phone_clicks_by_age_gender_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Call Now button, broken down by age and gender group.
*day, week, days_28*
##### page_call_phone_clicks_logged_in_by_country_unique
Number of unique people who logged in to Facebook and clicked the Call Now button, broken down by countries.
*day, week, days_28*
##### page_call_phone_clicks_logged_in_by_city_unique
Number of unique people who logged in to Facebook and clicked the Call Now button, broken down by city.
*day, week, days_28*
##### page_call_phone_clicks_by_site_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Call Now button, broken down by www, mobile, api
*day, week, days_28*
##### page_get_directions_clicks_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Get Directions button.
*day, week, days_28*
##### page_get_directions_clicks_by_age_gender_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Get Directions button, broken down by age and gender group.
*day, week, days_28*
##### page_get_directions_clicks_logged_in_by_country_unique
Number of unique people who logged in to Facebook and clicked the Get Directions button, broken down by country.
*day, week, days_28*
##### page_get_directions_clicks_logged_in_by_city_unique
Number of unique people who logged in to Facebook and clicked the Get Directions button, broken down by city.
*day, week, days_28*
##### page_get_directions_clicks_by_site_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Get Directions button, broken down by www, mobile, api or other.
*day, week, days_28*
##### page_website_clicks_logged_in_unique
Number of unique people who logged in to Facebook and clicked the goto website CTA button.
*day, week, days_28*
##### page_website_clicks_by_age_gender_logged_in_unique
Number of unique people who logged in to Facebook and clicked the goto website CTA button, broken down by age and gender group.
*day, week, days_28*
##### page_website_clicks_logged_in_by_country_unique
Number of unique people who logged in to Facebook and clicked the goto website CTA button, broken down by country.
*day, week, days_28*
##### page_website_clicks_logged_in_by_city_unique
Number of unique people who logged in to Facebook and clicked the goto website CTA button, broken down by city.
*day, week, days_28*
##### page_website_clicks_by_site_logged_in_unique
Number of unique people who logged in to Facebook and clicked the Page CTA button, broken down by www, mobile, api and other.
*day, week, days_28*

### Page User Demographics
##### page_fans
The total number of people who have liked your Page. A Page must have 30 or more fans for this metric to return data.
*lifetime*
##### page_fans_locale
Aggregated language data about the people who like your Page based on the default language setting selected when accessing Facebook.
*lifetime*
##### page_fans_city	
Aggregated Facebook location data, sorted by city, about the people who like your Page.
*lifetime*
##### page_fans_country	
The number of people, aggregated per country, that like your Page. Only the 45 countries with the most people that like your Page are included.
*lifetime*
##### page_fans_gender_age	
Aggregated demographic data about the people who like your Page based on the age and gender information they provide in their user profiles.
*lifetime*
##### page_fan_adds
The number of new people who have liked your Page.
*day*
##### page_fan_adds_unique
The number of new people who have liked your Page.
*day, week, days_28*
##### page_fans_by_like_source
This is a breakdown of the number of Page likes from the most common places where people can like your Page.
*day*

| Name | Description
| ------ | ------
| Ads | Page likes that came from people who saw your Page or post in an ad.
| News Feed | Page likes that came from people who saw content posted by your Page or about your Page in News Feed.
| Page Suggestions | Page likes that came from people saw your Page in a list of suggested Pages.
| Restored Likes from Reactivated Accounts | Page likes that came from people who reactivated their Facebook profile.
| Search | Page likes that came from people who saw you Page or post in search
| Your Page | Page likes that came from people who visited your Page.
##### page_fans_by_like_source_unique
The number of people who liked your Page, broken down by the most common places where people can like your Page.
*day*

| Name | Description
| ------ | ------
| Ads | Page likes that came from people who saw your Page or post in an ad.
| News Feed | Page likes that came from people who saw content posted by your Page or about your Page in News Feed.
| Page Suggestions | Page likes that came from people saw your Page in a list of suggested Pages.
| Restored Likes from Reactivated Accounts | Page likes that came from people who reactivated their Facebook profile.
| Search | Page likes that came from people who saw you Page or post in search
| Your Page | Page likes that came from people who visited your Page.
##### page_fan_removes
Unlikes of your Page.
*day*
##### page_fan_removes_unique
Number of people unliking your Page.
*day*
##### page_fans_by_unlike_source_unique
The number of people who unliked your Page, broken down by the most common ways people can unlike your Page.
*day*

### Page Content
Most of the metrics below can be retrieved using post_stories_by_action_type, post_consumptions_by_type, and page_consumptions_by_consumption_type.
##### page_tab_views_login_top_unique
The number of users logged in to Facebook who saw tabs on your Page.
*day, week*
##### page_tab_views_login_top
The number of times users logged in to Facebook saw tabs on your Page.
*day, week*
##### page_tab_views_logout_top
The number of times users not logged in to Facebook saw tabs on your Page.
*day*

| Name | Description
| ------ | ------
| allactivity | Administrative tab
| app | Custom created tab
| info | About tab view
| insights | Insights tab
| likes | Likes tab
| locations | Map tab
| photos | Photos tab
| photos_albums | Photos tab
| photos_stream | Photos tab
| profile | Pages timeline
| profile_info | Info tab
| profile_likes | Likes tab
| profile_photos |  Photos tab
| timeline | Pages timeline
| events | Events tab
| videos | Videos tab
| wall | Timeline

### Page Views
##### page_views_total	
The number of times a Page's profile has been viewed by logged in and logged out people.
*day, week, days_28*
##### page_views_logout
The number of times a Page's profile has been viewed by people not logged in to Facebook.
*day*
##### page_views_logged_in_total
The number of times a Page's profile has been viewed by people logged in to Facebook.
*day, week, days_28*
##### page_views_logged_in_unique
The number of people logged in to Facebook who have viewed the Page profile.
*day, week, days_28*
##### page_views_external_referrals
Top referrering external domains sending traffic to your Page.
*day*
##### page_views_by_profile_tab_total
The number of people who have viewed each Page profile tab.
*day, week, days_28*
##### page_views_by_profile_tab_logged_in_unique
The number of people logged in to Facebook who have viewed your Page's profile, broken down by each tab.
*day, week, days_28*
##### page_views_by_internal_referer_logged_in_unique
The number of people logged in to Facebook who have viewed your Page, broken down by the internal referer within Facebook.
*day, week, days_28*
##### page_views_by_site_logged_in_unique
The number of people logged in to Facebook who have viewed your Page profile, broken down by the type of device.
*day, week, days_28*
##### page_views_by_age_gender_logged_in_unique
The number of people logged in to Facebook who have viewed your Page profile, broken down by gender group.
*day, week, days_28*
##### page_views_by_referers_logged_in_unique
Logged-in page visit counts (unique users) by referral source.
*day, week, days_28*

### Page Video Views
##### page_video_views
Total number of times page's videos have been viewed for more than 3 seconds.
*day, week, days_28*
##### page_video_views_paid
Total number of times page's promoted videos have been viewed for more than 3 seconds.
*day, week, days_28*
##### page_video_views_organic
Total number of times page's videos have been viewed for more than 3 seconds by organic reach.
*day, week, days_28*
##### page_video_views_by_paid_non_paid
Total number of times page's videos have been viewed for more than 3 seconds, broken down by total, paid and non-paid.
*day, week, days_28*
##### page_video_views_autoplayed
Total number of times page's autoplayed videos have been viewed for more than 3 seconds.
*day, week, days_28*
##### page_video_views_click_to_play
Total number of times page's videos have been viewed after the user clicks on play for more than 3 seconds.
*day, week, days_28*
##### page_video_views_unique
Total number of times page's videos have been played for unique people for more than 3 seconds.
*day, week, days_28*
##### page_video_repeat_views
Total number of times that people replay a page's videos for more than 3 seconds.
*day, week, days_28*
##### page_video_complete_views_30s
Total number of times page's videos have been viewed for more than 30 seconds.
*day, week, days_28*
##### page_video_complete_views_30s_paid
Total number of times page's promoted videos have been viewed to the end, or for more than 30 seconds.
*day, week, days_28*
##### page_video_complete_views_30s_organic
Total number of times page's videos have been viewed to the end, or viewed for more than 30 seconds by organic reach.
*day, week, days_28*
##### page_video_complete_views_30s_autoplayed
Total number of times page's autoplayed videos have been viewed to the end, or viewed for more than 30 seconds.
*day, week, days_28*
##### page_video_complete_views_30s_click_to_play
Total number of times page's videos have been viewed to the end, or viewed after the user clicks on play for more than 30 seconds.
*day, week, days_28*
##### page_video_complete_views_30s_unique
Total number of times page's videos have been played for unique people to the end, or viewed for more than 30 seconds.
*day, week, days_28*
##### page_video_complete_views_30s_repeat_views
Total number of times that people replay a page's videos to the end, or for more than 30 seconds.
*day, week, days_28*
##### post_video_complete_views_30s_autoplayed
Number of times your video started automatically playing and people viewed it for 30 seconds or to the end, whichever came first. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_30s_clicked_to_play
Number of times people clicked to play your video and viewed it for 30 seconds or to the end, whichever came first. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_30s_organic
Number of times your video was viewed for 30 seconds or viewed to the end, whichever came first, without a paid promotion. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_30s_paid
Number of times your video was viewed for 30 seconds or viewed to the end, whichever came first, after a paid promotion. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_30s_unique
Total number of times page's videos have been viewed for more than 30 seconds by unique users. Returns 0 for reshared videos.
*lifetime*
##### page_video_views_10s
The number of times your Page's videos were watched for an aggregate of at least 10 seconds, or for nearly its total length, whichever happened first.
*day, week, days_28*
##### page_video_views_10s_paid
The number of times your Page's videos with paid activity were watched for at least a total of 10 seconds, or for nearly their total length, whichever happened first.
*day, week, days_28*
##### page_video_views_10s_organic
The number of times your Page's videos were watched without any paid distribution for at least a total of 10 seconds, or for nearly their total length, whichever happened first.
*day, week, days_28*
##### page_video_views_10s_autoplayed
The number of times your Page's videos were started automatically and watched for at least a total of 10 seconds, or for nearly their total length, whichever happened first.
*day, week, days_28*
##### page_video_views_10s_click_to_play
The number of times your Page's videos were started by clicking the play button and watched for at least a total of 10 seconds, or for nearly their total length, whichever happened first.
*day, week, days_28*
##### page_video_views_10s_unique
The number of times your Page's videos were watched for an aggregate of at least 10 seconds, or for nearly its total length, whichever happened first, by unique users.
*day, week, days_28*
##### page_video_views_10s_repeat
The number of times your Page's videos were replayed for at least 10 seconds, or for nearly its total length, whichever happened first.
*day, week, days_28*
##### page_video_view_time
The total amount of time (in milliseconds) people spent watching videos on your Page.
*day*

### Page Posts
##### page_posts_impressions*
The number of times your Page's posts entered a person's screen. Posts include statuses, photos, links, videos and more.
*day, week, days_28*
##### page_posts_impressions_unique*	
The number of people who had any of your Page's posts enter their screen. Posts include statuses, photos, links, videos and more.
*day, week, days_28*
##### page_posts_impressions_paid*
The number of times your Page's posts entered a person's screen through paid distribution such as an ad.
*day, week, days_28*
##### page_posts_impressions_paid_unique*
The number of people who had any of your Page's posts enter their screen through paid distribution such as an ad.
*day, week, days_28*
##### page_posts_impressions_organic*	
The number of times your Page's posts entered a person's screen through unpaid distribution.
*day, week, days_28*
##### page_posts_impressions_organic_unique*	
The number of people who had any of your Page's posts enter their screen through unpaid distribution.
*day, week, days_28*
##### page_posts_served_impressions_organic_unique		
The number of people who were served your Page's posts in their News Feed whether it entered their screen or not. Posts include statuses, photos, links, videos and more.
*day, week, days_28*
##### page_posts_impressions_viral*	
The number of times your Page's posts entered a person's screen with social information attached. Social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_posts_impressions_viral_unique*	
The number of people who had any of your Page's posts enter their screen with social information attached. As a form of organic distribution, social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_posts_impressions_nonviral*	
The number of times your Page's posts entered a person's screen. This does not include content created about your Page with social information attached. Social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_posts_impressions_nonviral_unique*	
The number of people who had any posts by your Page enter their screen. This does not include content created about your Page with social information attached. As a form of organic distribution, social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*day, week, days_28*
##### page_posts_impressions_frequency_distribution	
The number of people who saw your Page posts, broken down by how many times people saw your posts.
*day, week, days_28*

## Single Post Stats
### Page Post Impressions
Note that the unique impression insights values are calculated independently. Total page reach may not always be exactly equal to the sum of paid and non-paid unique values.
##### post_impressions*
The number of times your Page's post entered a person's screen. Posts include statuses, photos, links, videos and more.
*lifetime*
##### post_impressions_unique*
The number of people who had your Page's post enter their screen. Posts include statuses, photos, links, videos and more.
*lifetime*
##### post_impressions_paid*
The number of times your Page's post entered a person's screen through paid distribution such as an ad.
*lifetime*
##### post_impressions_paid_unique*	
The number of people who had your Page's post enter their screen through paid distribution such as an ad.
*lifetime*
##### post_impressions_fan*
The number of impressions for your Page post by people who have liked your Page.
*lifetime*
##### post_impressions_fan_unique*
The number of people who have like your Page who saw your Page post.
*lifetime*
##### post_impressions_fan_paid*	
The number of impressions for your Page post by people who like your Page in an Ad or Sponsored Story.
*lifetime*
##### post_impressions_fan_paid_unique*	
The number of people who have like your Page and saw your Page post in an Ad or Sponsored Story.
*lifetime*
##### post_impressions_organic*
The number of times your Page's posts entered a person's screen through unpaid distribution.
*lifetime*
##### post_impressions_organic_unique*	
The number of people who had your Page's post enter their screen through unpaid distribution.
*lifetime*
##### post_impressions_viral*
The number of times your Page's post entered a person's screen with social information attached. Social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*lifetime*
##### post_impressions_viral_unique*	
The number of people who had your Page's post enter their screen with social information attached. As a form of organic distribution, social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*lifetime*
##### post_impressions_nonviral*	
The number of times your Page's post entered a person's screen. This does not include content created about your Page with social information attached. Social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*lifetime*
##### post_impressions_nonviral_unique*	
The number of people who had your Page's post enter their screen. This does not include content created about your Page with social information attached. As a form of organic distribution, social information displays when a person's friend interacted with you Page or post. This includes when someone's friend likes or follows your Page, engages with a post, shares a photo of your Page and checks into your Page.
*lifetime*
##### post_impressions_by_story_type*	
The number of times this post was seen via a story published by a friend of the person viewing the post.
*lifetime*
##### post_impressions_by_story_type_unique*	
The number of people who saw your page post in a story from a friend, by story type.
*lifetime*

### Page Post Engagement
##### post_engaged_users*
The number of people who clicked anywhere in your posts.
*lifetime*
##### post_negative_feedback*
The number of times people took a negative action in your post (e.g. hid it).
*lifetime
##### post_negative_feedback_unique*	
The number of people who took a negative action in your post (e.g., hid it).
*lifetime*
##### post_negative_feedback_by_type*	
The number of times people took a negative action in your post broken down by type.
*lifetime*
##### post_negative_feedback_by_type_unique*	
The number of people who took a negative action in your post broken down by type.
*lifetime*
##### post_engaged_fan
People who have liked your page and engaged with your post.
*lifetime*
##### post_clicks*
The number of times people clicked on anywhere in your posts without generating a story.
*lifetime*
##### post_clicks_unique*
The number of people who clicked anywhere in your post without generating a story.
*lifetime*
##### post_clicks_by_type*
The number of times people clicked on anywhere in your posts without generating a story, by consumption type.
*lifetime*
##### post_clicks_by_type_unique*	
The number of people who clicked anywhere in your post without generating a story, by consumption type.
*lifetime*

### Page Post Reactions
##### post_reactions_like_total
Total "like" reactions of a post.
*lifetime*
##### post_reactions_love_total
Total "love" reactions of a post.
*lifetime*
##### post_reactions_wow_total
Total "wow" reactions of a post.
*lifetime*
##### post_reactions_haha_total
Total "haha" reactions of a post.
*lifetime*
##### post_reactions_sorry_total
Total "sorry" reactions of a post.
*lifetime*
##### post_reactions_anger_total
Total "anger" reactions of a post.
*lifetime*
##### post_reactions_by_type_total	
Total post reactions by type.
*lifetime*

### Page Video Posts
##### post_video_avg_time_watched
The average length of time (in milliseconds) people spent viewing your video. Only available for videos created after August 25th 2016. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_organic	
The number of times your video was organically viewed from the beginning to 95% of its length. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_organic_unique	
The number of people who viewed your video organically from the beginning to 95% of its length. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_paid
The number of times your video was viewed via paid impression from the beginning to 95% of its length. Returns 0 for reshared videos.
*lifetime*
##### post_video_complete_views_paid_unique	
The number of people who viewed your video via paid impression from the beginning to 95% of its length. Returns 0 for reshared videos.
*lifetime*
##### post_video_retention_graph*
Views of your video at each interval as a percentage of all views. This metric does not count views of videos while they were live. Retention graphs may show more viewers later in the video than at the beginning. People might start the video in the middle, skip ahead, save and rewatch it from that point, or other similar behaviors.
*lifetime*
##### post_video_retention_graph_clicked_to_play	
Clicked-to-play views of your video at each interval as a percentage of all clicked-to-play views. This metric does not count views of videos while they were live. Retention graphs may show more viewers later in the video than at the beginning. People might start the video in the middle, skip ahead, save and rewatch it from that point, or other similar behaviors.
*lifetime*
##### post_video_retention_graph_autoplayed
Auto-played views of your video at each interval as a percentage of all auto-played views. This metric does not count views of videos while they were live. Retention graphs may show more viewers later in the video than at the beginning. People might start the video in the middle, skip ahead, save and rewatch it from that point, or other similar behaviors.
*lifetime*
##### post_video_views_organic
The number of times your video was organically viewed for 3 seconds or more.
*lifetime*
##### post_video_views_organic_unique
The number of people who viewed at least 3 seconds of your video organically.
*lifetime*
##### post_video_views_paid
The number of times your video was viewed via paid impression for 3 seconds or more.
*day, lifetime*
##### post_video_views_paid_unique
The number of people who viewed at least 3 seconds of your video via paid impression.
*lifetime*
##### post_video_length
Length of a video post (in milliseconds).
*lifetime*
##### post_video_views
The number of times your video was watched for an aggregate of at least 3 seconds, or for nearly its total length, whichever happened first.
*day, lifetime*
##### post_video_views_unique
The number of distinct people who viewed your video at least once.
*lifetime*
##### post_video_views_autoplayed
Number of times your video started automatically playing and people viewed it for more than 3 seconds.
*lifetime*
##### post_video_views_clicked_to_play
Number of times people clicked to play your video and viewed it more than 3 seconds.
*lifetime*
##### post_video_views_10s
The number of times your video was watched for an aggregate of at least 10 seconds, or for nearly its total length, whichever happened first. Returns 0 for reshared videos.
*lifetime*
##### post_video_views_10s_unique
Number of unique viewers who watched your video for 10 seconds or to the end, whichever happened first. Returns 0 for reshared videos.
*lifetime*
##### post_video_views_10s_autoplayed
Number of times your video started playing automatically and people viewed it for 10 seconds or to the end, whichever happened first. Returns 0 for reshared videos.
*lifetime*
##### post_video_views_10s_clicked_to_play
Number of times people clicked to play your video and viewed it for 10 seconds or to the end, whichever happened first. Returns 0 for reshared videos.
*lifetime*
##### post_video_views_10s_organic
Number of times your video was viewed with sound on for 10 seconds or viewed to the end, whichever happened first. Returns 0 for reshared videos.
*lifetime*
##### post_video_views_sound_on
Number of times your video was viewed with sound on for 3 seconds or viewed to the end, whichever happened first.
*lifetime*
##### post_video_view_time
The total number of milliseconds your video was watched, including replays and views less than 3 seconds. Returns 0 for reshared videos.
*day, lifetime*
##### post_video_view_time_organic
Total time (in milliseconds) video has been viewed without paid promotion. Returns 0 for reshared videos.
*day, lifetime*
##### post_video_view_time_by_age_bucket_and_gender
Total time (in milliseconds) video has been viewed by Top Audiences.
*lifetime*
##### post_video_view_time_by_region_id
Total time (in milliseconds) video has been viewed by Top 45 Locations (Region ##### Country).
*lifetime*
##### post_video_views_by_distribution_type
Number of times your video was viewed by distribution type (page_owned and shared).
*lifetime*
##### post_video_view_time_by_distribution_type
Total time (in milliseconds) video has been viewed by distribution type (page_owned and shared).
*lifetime*
##### post_video_view_time_by_country_id
Total time (in minutes) video has been viewed by Top 45 Locations (Country).
*lifetime*

### Video Ad Breaks
##### page_daily_video_ad_break_ad_impressions_by_crosspost_status
Number of times an ad was shown during ad breaks in a crossposted video.
*day*
##### page_daily_video_ad_break_cpm_by_crosspost_status
Average amount paid by advertisers for 1,000 impressions of their ads in a crossposted video. This is a gross number and includes the amount paid to Facebook.
*day*
##### page_daily_video_ad_break_earnings_by_crosspost_status
An estimate of the amount you earned from ad breaks in a crossposted video, based on the number of impressions and CPM of ads shown. Actual payments may differ if there are content ownership claims or other adjustments.
*day*
##### post_video_ad_break_ad_impressions
Number of times an ad was shown during ad breaks in the video attached to the post.
*day, lifetime*
##### post_video_ad_break_earnings
An estimate of the amount you earned from ad breaks in the video attached to the post, based on the number of impressions and CPM of ads shown. Actual payments may differ if there are content ownership claims or other adjustments.
*day, lifetime*
##### post_video_ad_break_ad_cpm
Average amount paid by advertisers for 1,000 impressions of their ads in the video attached to the post. This number also includes the amount paid to Facebook
*day, lifetime*
