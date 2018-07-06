# Youtube Insights

Youtube insights are not served with specific calls, you have to generate queries to get the data you are interested in.
The data is caracterised by metrics(the measurement like views, likes and dislikes) and dimensions(the criteria to aggregate data, like country or date).
You can then specify filters to have a limited set of answers.

## Metrics
### Views metrics
##### views
The number of times that a video was viewed. In a playlist report, the metric indicates the number of times that a video was viewed in the context of a playlist.
##### red_views
The number of times that a video was viewed by YouTube Red members.
##### views_percentage
The percentage of viewers who were logged in when watching the video or playlist.

### Watch time metrics
##### watch_time_minutes
The number of minutes that users watched videos for the specified channel, content owner, video, or playlist.
##### red_watch_time_minutes
The number of minutes that YouTube Red members watched a video.
##### average_view_duration_seconds
The average length, in seconds, of video playbacks. In a playlist report, the metric indicates the average length, in seconds, of video playbacks that occurred in the context of a playlist. 
##### average_view_duration_percentage
The average percentage of a video watched during a video playback.

### Engagement metrics
##### comments
The number of times that users commented on a video.
##### likes
The number of times that users indicated that they liked a video by giving it a positive rating.
##### dislikes
The number of times that users indicated that they disliked a video by giving it a negative rating.
##### shares
The number of times that users shared a video through the Share button.
##### subscribers_gained
The number of times that users subscribed to a channel.
##### subscribers_lost
The number of times that users unsubscribed from a channel.
##### videos_added_to_playlists
The number of times that videos were added to any YouTube playlists. The videos could have been added to the video owner's playlist or to other channels' playlists.
##### videos_removed_from_playlists
The number of times that videos were removed from any YouTube playlists. The videos could have been removed from the video owner's playlist or from other channels' playlists.

### Playlist metrics
##### playlist_starts
The number of times that viewers initiated playback of a playlist. Note that this metric only includes playlist views that occurred on the web.
##### playlist_saves_added
(only supported in YouTube Reporting API)
The number of times that users saved a playlist.
##### playlist_saves_removed
(only supported in YouTube Reporting API)
The number of times that users removed the playlist from their lists of saved playlists.

### Annotations metrics
##### annotation_impressions
The total number of annotation impressions.
##### annotation_clickable_impressions
The number of annotations that appeared and could be clicked.
##### annotation_clicks
The number of clicked annotations.
##### annotation_click_through_rate
The ratio of annotations that viewers clicked to the total number of clickable annotation impressions. 
##### annotation_closable_impressions
The number of annotations that appeared and could be closed.
##### annotation_closes
The number of closed annotations.
##### annotation_close_rate
The ratio of annotations that viewers closed to the total number of annotation impressions. 

### Card metrics
##### card_impressions
The number of times cards were displayed. When the card panel is opened, a card impression is logged for each of the video's cards.
##### card_clicks
The number of times that cards were clicked.
##### card_click_rate
The click-through-rate for cards, which is calculated as the ratio of card clicks to card impressions.
##### card_teaser_impressions
The number of times that card teasers were displayed. A video view can generate multiple teaser impressions.
##### card_teaser_clicks
The number of clicks on card teasers. Card icon clicks are attributed to the last teaser displayed to the user.
##### card_teaser_click_rate
The click-through-rate for card teasers, which is calculated as the ratio of clicks on card teasers to the total number of card teaser impressions.

### End screen metrics
End screens are elements that show during the last five to 20 seconds of a video to promote your content, channel, and websites.
##### end_screen_element_impressions
The number of end screen elements that were displayed. One impression is logged for each end screen element that displays.
##### end_screen_element_clicks
The number of times that end screen elements were clicked.
##### end_screen_element_click_rate
The click-through-rate for end screen elements, which is calculated as the ratio of end screen element clicks to end screen element impressions.

### Audience retention metrics
##### audience_retention_percentage
The absolute ratio of viewers watching the video at the given point in the video. The ratio is calculated by comparing the number of times a portion of a video has been watched to the total number of views of the video. The elapsed_video_time_percentage dimension identifies the portion of the video to which the metric corresponds.

Note that a portion of a video could be watched more than once (or not at all) in a given video view. For example, if users rewind and watch the same portion of a video multiple times, then the absolute ratio for that portion of the video the could be greater than 1.

The following examples illustrate how the value is calculated:
- A one-minute video is watched 100 times. Half of the viewers stop watching after 15 seconds and the rest watch the entire video. None of the viewers watch any parts of the video more than once. In this case, this metric's value would be 1 for time buckets in the first quarter of the video, and its value would be 0.50 for the remainder of the video.
- A one-minute video is watched 100 times. All of the viewers watch the entire video, but 20 of the viewers watch until the video's 45-second mark, then skip back to the video's 30-second mark, and then watch the remainder of the video. In this case, the metric's value would be 1 for time buckets in either the first half or the last quarter of the video. However, the value would be 1.2 for time buckets in the third quarter of the video since 100 percent of the viewers watched that segment of the video but 20% of those viewers watched the segment twice.

### Earnings metrics
##### estimated_partner_revenue
The total estimated earnings (net revenue) from all Google-sold advertising sources as well as from non-advertising sources for the selected date range and region. 
##### estimated_partner_ad_revenue
The total estimated earnings (net revenue) from all Google-sold advertising sources for the selected date range and region.

Estimated earnings are subject to month-end adjustment and do not include partner-sold and partner-served advertising.
##### estimated_partner_ad_auction_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from auction-sold advertising via AdSense for the selected date range and region. This metric was previously named estimated_partner_ad_sense_revenue.
##### estimated_partner_ad_sense_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from auction-sold AdSense advertising for the selected date range and region.
##### estimated_partner_ad_reserved_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from reserved-sold advertising via DoubleClick (DCLK) and other YouTube-sold sources. This metric was previously named estimated_partner_double_click_revenue.
##### estimated_partner_double_click_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from reserved-sold advertising via DoubleClick (DCLK) and other YouTube-sold sources.

Note: This metric has been renamed and is called estimated_partner_ad_reserved_revenue in the most current versions of all reports that contain it.
##### estimated_partner_ad_reserved_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from reserved-sold advertising via DoubleClick (DCLK) and other YouTube-sold sources. This metric was previously named estimated_partner_double_click_revenue.
##### estimated_partner_double_click_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from reserved-sold advertising via DoubleClick (DCLK) and other YouTube-sold sources.

Note: This metric has been renamed and is called estimated_partner_ad_reserved_revenue in the most current versions of all reports that contain it.
##### estimated_partner_red_revenue
(only supported in YouTube Reporting API)
The total estimated earnings (net revenue) from YouTube Red subscriptions.
##### estimated_partner_transaction_revenue
(only supported in YouTube Reporting API)
The total estimated revenue from transactions, such as paid content and Fan Funding, minus any partner-charged refunds.

### Ad performance metrics
##### estimated_youtube_ad_revenue
The estimated gross revenue, in USD, from all Google-sold or DoubleClick-partner-sold advertising for the selected date range and region. Gross revenue is subject to month-end adjustment and does not include partner-served advertising. Gross revenue should not be confused with earnings, or net revenue, which factors in your share of ownership and revenue-sharing agreements.
##### estimated_cpm
The estimated gross revenue per thousand ad impressions.
##### ad_impressions
The number of verified ad impressions served.
##### estimated_monetized_playbacks
The number of instances when a viewer played your video and was shown at least one ad impression. A monetized playback is counted if a viewer is shown a preroll ad but quits watching the ad before your video ever starts. The expected estimated error for this figure is ±2.0%.
##### estimated_playback_based_cpm
The estimated gross revenue per thousand playbacks.

## Dimensions
### Resources
These dimensions correspond to resources that channels and content owners manage on YouTube.
##### video_id
The ID of a YouTube video. In the YouTube Data API, this is the value of a video resource's id property.
##### playlist_id
The ID of a YouTube playlist. In the YouTube Data API, this is the value of a playlist resource's id property.
##### channel_id
The ID for a YouTube channel. In the YouTube Data API, this is the value of a channel resource's id property.
##### asset_id
The ID of an asset managed in YouTube's Content ID system. An asset is the representation of your intellectual property in that system. On the YouTube website, you can locate asset IDs in YouTube Content Manager. You can also retrieve them using the YouTube Content ID API.

### Geographic areas
These dimensions identify a geographic region associated with user activity, ad performance, or estimated revenue metrics.
##### country_code
The country associated with the metrics in the report row. The dimension value is a two-letter ISO-3166-1 country code, such as US, CN (China), or FR (France). The country code ZZ is used to report metrics for which YouTube could not identify the associated country.
##### province_code
The U.S. state or territory associated with the metrics in the report row. The dimension values is an ISO 3166-2 code that identifies a U.S. state or the District of Columbia, such as US-MI (Michigan) or US-TX (Texas). The province code US-ZZ is used to report metrics for which YouTube could not identify the associated U.S. state.

Note: This dimension does not support ISO 3166-2 values that identify U.S. outlying areas since those territories also have their own ISO 3166-1 country codes. It also does not support subdivisions of countries other than the United States.

### Time periods
##### date
This dimension identifies the date associated with the metrics in each report row. In bulk reports, the date refers to the period beginning at 12:00 a.m. Pacific time and ending at 11:59 p.m. Pacific time on the specified day, month, and year. Depending on the time of year, Pacific time is either UTC-7 or UTC-8.

Note that while dates typically represent a 24-hour period, dates when clocks are adjusted forward for Daylight Savings Time represent a 23-hour period, and dates when clocks are adjusted backward represent a 25-hour period.

### Playback locations
##### playback_location_type
This dimension identifies the type of page or application where user activity occurred. The following table lists dimension values:
| Values | Description
| ------ | ------
| 0 | The data pertains to activity that occurred on the video's YouTube watch page or in an official YouTube application, such as the YouTube Android app.
| 1 | The data pertains to activity that occurred on another website or application where the video was embedded using an \<iframe> or \<object> embed.
| 2 |The data pertains to activity that occurred on a YouTube channel page.
| 5 | The data pertains to metrics that cannot be classified into one of the other location types listed above.
| 7 | The data pertains to views that took place on the YouTube home page or home screen, in the user's subscription feed, or in another YouTube browsing feature.
| 8 | The data pertains to views that took place directly on the YouTube search results page.
##### playback_location_detail
This dimension specifies the URL or application where the playback occurred. This dimension is only supported for views that occurred in embedded players, which means that the dimension value is only populated in rows where the dimension's value is 1. In other rows, this dimension's value is empty.

### Playback details
##### live_or_on_demand
This dimension indicates whether the user activity metrics in the data row are associated with views of a live broadcast. Data for this dimension is available for dates beginning April 1, 2014.

The following table lists dimension values:
| Values | Description
| ------ | ------
| live | The row's data describes user activity that occurred during a live broadcast.
| onDemand | The row's data describes user activity that did not occur during a live broadcast.
##### subscribed_status
This dimension indicates whether the user activity metrics in the data row are associated with viewers who were subscribed to the video's or playlist's channel. Possible values are subscribed and unsubscribed.
Note that the dimension value is accurate as of the time that the user activity occurs. For example, suppose a user has not subscribed to a channel and watches one of that channel's videos, then subscribes to the channel and watches another video, all on the same day. The channel's report indicates that one view has a subscribed_status value of subscribed, and one view has a subscribed_status value of unsubscribed.

### Traffic sources
##### traffic_source_type
This dimension identifies the referrer type associated with the user activity metrics. The referrer type describes the manner in which users reached the video or channel associated with the row of data in the report. The following table lists dimension values:
| Values | Description
| ------ | ------
| 0 |  	*Direct or unknown* This value encompasses direct traffic to a page as well as pages for which the referrer is unknown. In query reports, this traffic source type is identified as NO_LINK_OTHER or UNKNOWN_MOBILE_OR_DIRECT.
| 1 | *YouTube advertising* The viewer was referred to the video by an advertisement. In a traffic source report, if this dimension's value is 1, then the traffic_source_detail dimension identifies the type of advertisement that was shown to the viewer. In query reports, this traffic source type is identified as ADVERTISING. 
| 3 | *Browse features* The viewer was referred from a YouTube page that leads to videos or channels. In a traffic source report, if this dimension's value is 3, then the traffic_source_detail dimension identifies the feature that referred the traffic. In query reports, this traffic source type is identified as SUBSCRIBER.
| 4 | *YouTube channels* Viewers were referred from a YouTube channel page. In a traffic source report, if this dimension's value is 4, then the traffic_source_detail dimension specifies the channel ID for that channel. In query reports, this traffic source type is identified as YT_CHANNEL.
| 5 | *YouTube search* Viewers were referred from YouTube search results. In a traffic source report, if this dimension's value is 5, then the traffic_source_detail dimension specifies the associated search term. In query reports, this traffic source type is identified as YT_SEARCH.
| 7 | *Suggested videos* Viewers were referred from a related video listing on another video watch page. In a traffic source report, if this dimension's value is 7, then the traffic_source_detail dimension identifies the video ID for that video. In query reports, this traffic source type is identified as RELATED_VIDEO or YT_RELATED.
| 8 | *Other YouTube features* Viewers were referred from a YouTube page that does not fall into one of the other listed traffic source types. In a traffic source report, if this dimension's value is 8, then the traffic_source_detail dimension identifies the page URL. In query reports, this traffic source type is identified as YT_OTHER_PAGE.
| 9 | *External* Viewers were referred from a link on another website. This traffic source includes referrals from Google search results. In a traffic source report, if this dimension's value is 9, then the traffic_source_detail dimension identifies the external web page. In query reports, this traffic source type is identified as EXT_URL.
| 11 | *Video cards and annotations* Viewers were referred by clicking on an annotation or card in another video. In query reports, this traffic source type is identified as ANNOTATION.
| 14 | *Playlists* Views occurred while the video was being played as part of a playlist. In query reports, this traffic source type is identified as PLAYLIST. Note that this traffic source differs from source type 18, which indicates that the views originated from the page that lists all of the videos in the playlist.
| 17 | *Notifications* Viewers were referred from an email or notification from YouTube. In query reports, this traffic source type is identified as NOTIFICATION.
| 18 | *Playlist pages* Views originated from a page that lists all of the videos in a playlist. In query reports, this traffic source type is identified as YT_PLAYLIST_PAGE. Note that this traffic source differs from source type 14, which indicates that the views occurred while the video was being played as part of a playlist.
| 19 | *Programming from claimed content* Views originated from claimed, user-uploaded videos that the content owner used to promote the viewed content. In query reports, this traffic source is identified as CAMPAIGN_CARD. This traffic source is only supported for content owner reports.
| 20 | *Interactive video endscreen* Views originated from the endscreen of another video. In query reports, this traffic source type is identified as END_SCREEN.
##### traffic_source_detail
This dimension provides additional detail about the traffic source that the row's traffic_source_type dimension value. This dimension value is populated for the following traffic_source_type dimension values:
| Values | Description
| ------ | ------
| 1 | The dimension value identifies the type of advertisement that was shown to the viewer. See the traffic_source_type definition for a list of possible values.
| 3 | The dimension value identifies the YouTube feature that led to the referred traffic. See the traffic_source_type definition for a list of possible values.
| 4 | The dimension value specifies the channel ID from which the viewer was referred.
| 5 | The dimension value specifies the search term that led to the referred traffic.
| 7 | The dimension value identifies the video from which the viewer was referred.
| 8 | The dimension value identifies the type of YouTube page that led to the referred traffic. See the traffic_source_type definition for a list of possible values.
| 9 | The dimension value identifies the external page from which the traffic was referred.
| 17 | The dimension value identifies the type of notification that led to the referred traffic. See the traffic_source_type definition for a list of possible values.
| 19 | The dimension value identifies the video from which the viewer was referred.
| 20 | The dimension value identifies the video from which the viewer was referred.

### Devices
##### device_type
This dimension identifies the physical form factor of the device on which the view occurred. The following table lists valid dimension values:
| Values | Description
| ------ | ------
| 100 | Unknown
| 101 | Computer
| 102 | TV
| 103 | Game console
| 104 | Mobile phone
| 105 | Tablet
##### operating_system
This dimension identifies the software system of the device on which the view occurred. The following table lists valid dimension values:
| Values | Description
| ------ | ------
| 1 | Other
| 2 | Windows
| 3 | Windows Mobile
| 4 | Android
| 5 | iOS
| 6 | Symbian
| 7 | Blackberry
| 9 | Macintosh
| 10 | PlayStation
| 11 | Bada
| 12 | WebOS
| 13 | Linux
| 14 | Hiptop
| 15 | MeeGo
| 16 | Wii
| 17 | Xbox
| 18 | PlayStation Vita
| 19 | Smart TV
| 20 | Nintendo 3DS
| 21 | Chromecast
| 22 | Tizen
| 23 | Firefox
| 24 | RealMedia
| 25 | KaiOS

### Demographics
Demographic dimensions help you to understand the age range and gender distribution of your audience. The YouTube Help Center contains additional information about demographic data in YouTube Analytics reports.
##### age_group
This dimension identifies the age group of the logged-in users associated with the report data. The API uses the following age groups:
- AGE_13_17
- AGE_18_24
- AGE_25_34
- AGE_35_44
- AGE_45_54
- AGE_55_64
- AGE_65_
##### gender
This dimension identifies the gender of the logged-in users associated with the report data. Valid values are FEMALE, MALE, and GENDER_OTHER.

Note that the YouTube Analytics API currently only returns the values female and male. As such, you may see some discrepancy in the views_percentage metric values that the two APIs return. (In the YouTube Analytics API, views_percentage is called viewerPercentage.)

### Engagement and content sharing
##### sharing_service
This dimension identifies the service that was used to share videos. Videos can be shared on YouTube (or via the YouTube player) using the "Share" button.
The following table lists valid dimension values:
| Values | Description
| ------ | ------
| 0 | Unknown
| 1 | Digg
| 4 | reddit
| 5 | StumbleUpon
| 6 | mixi
| 7 | Yahoo! Japan
| 8 | goo
| 9 | Ameba
| 10 | Facebook
| 11 | Myspace
| 12 | NUjij
| 18 | Tuenti
| 20 | menéame
| 21 | Wykop
| 22 | Skyrock
| 25 | Fotka
| 28 | hi5
| 31 | Twitter
| 32 | Cyworld
| 34 | Blogger
| 36 | VKontakte (ВКонтакте)
| 37 | Rakuten (楽天市場)
| 38 | LiveJournal
| 39 | Odnoklassniki (Одноклассники)
| 40 | tumblr.
| 42 | Linkedin
| 43 | Google+
| 44 | Weibo
| 45 | Pinterest
| 46 | Email
| 47 | Facebook Messenger
| 49 | WhatsApp
| 50 | Hangouts
| 51 | Gmail
| 52 | Kakao (Kakao Talk)
| 53 | Other
| 55 | Copy to Clipboard
| 59 | Embed
| 60 | Text message
| 61 | Android messaging
| 62 | Verizon messages
| 63 | HTC text message
| 64 | Sony Conversations
| 65 | Go SMS
| 66 | LGE Email
| 67 | Line
| 68 | Viber
| 69 | Kik
| 70 | Skype
| 71 | Blackberry Messenger
| 72 | WeChat
| 73 | KAKAO Story
| 74 | Dropbox
| 75 | Telegram
| 76 | Facebook Pages
| 77 | GroupMe
| 78 | Android Email
| 79 | Motorola Messaging
| 80 | Nearby Share
| 81 | Naver
| 82 | iOS System Activity Dialog
| 83 | Google Inbox
| 84 | Android Messenger
| 85 | YouTube Music
| 86 | YouTube Gaming
| 87 | YouTube Kids
| 88 | YouTube TV

### Annotations
##### annotation_type
This dimension identifies the manner in which the annotation displays during the video. The following table lists possible dimension values:
| Values | Description
| ------ | ------
| 0 | Unknown
| 1 | Note
| 3 | Spotlight
| 4 | Title
| 8 | Speech bubble
| 9 | Label
| 10 | Branding watermark
| 11 | Featured video
| 12 | Featured playlist
| 30 | Call-to-Action
##### annotation_id
The ID that YouTube uses to uniquely identify an annotation.

### Cards
##### card_type
This dimension identifies the type of card that was displayed to the user. The following table lists possible dimension values:
| Values | Description
| ------ | ------
| 0 | Unknown
| 60 | Link
| 61 | Fundraising
| 62 | Video 
| 63 | Playlist
| 65 | Fan Funding
| 66 | Merchandise
| 68 | Associated website
| 69 | Channel
##### card_id
The ID that YouTube uses to uniquely identify a card.

### End screens
##### end_screen_element_type
This dimension identifies the type of end screen element that was displayed to the user. The following table lists the end screen element types and their values:
| Values | Description
| ------ | ------
| 501 | Video - The element promotes another YouTube video.
| 502 | Playlist - The element promotes YouTube playlist.
| 503 | Website - The element links to your associated website.
| 504 | Channel - The element links to another channel.
| 505 | Subscribe - The element encourages subscriptions to your channel.
| 506 | Associated
| 507 | Crowdfunding - The element links to an approved crowdfunding website.
| 508 | Merchandise - The element links to an approved merchandise website.
| 509 | Recent upload - The element links to your channel's most recently uploaded video.
| 510 | Best for viewer
##### end_screen_element_id
The ID that YouTube uses to uniquely identify an end screen element.

### Subtitles
##### subtitle_language
This dimension identifies the closed caption language used for the longest time during the view. Views for which closed captions were mostly turned off are not counted. See the documentation for channel reports or content owner reports for more information about reports that contain this dimension.

### Ad performance
##### ad_type
The ad_type dimension is used in ad performance reports and aggregates the requested metrics based on the types of ads that ran during video playbacks. The following table lists possible dimension values.
| Values | Description | Value in Query Reports
| ------ | ------ | ------
| 1 | Skippable video ads (Auction) | auctionTrueviewInstream
| 2 | Display ads (Auction) | auctionDisplay
| 3 | Non-skippable video ads (Auction) | auctionInstream
| 5 | Display ads (Reserved) | reservedDisplay
| 6 | Non-skippable video ads (Reserved) | reservedInstream
| 13 | Unknown | unknown
| 15 | Skippable video ads (Reserved) | reservedInstreamSelect
| 19 | Bumper ads (auction) | auctionBumperInstream
| 20 | Bumper ads (reserved) | reservedBumperInstream
Note: Query reports might return for some additional ad types that were previously used on YouTube.

### Content owner dimensions
The following dimensions are only used in content owner reports.
##### claimed_status
(only used in content owner reports)
This dimension indicate that a row of data only contains metrics for claimed content. The only valid value for this dimension is claimed. The table in the definition of the uploader_type dimension provides more detail about how to use this dimension.
##### uploader_type
(only used in content owner reports)
This dimension indicates whether a row of data contains metrics for content uploaded by the specified content owner and/or content uploaded by third parties, such as user-uploaded videos. Valid values are self and thirdParty.
The table below shows the supported combinations for the claimed_status and uploader_type dimensions:
| claimed_status | uploader_type | Description
| ------ | ------ | ------
| [Not set] | self | The row contains YouTube Analytics data for claimed and unclaimed content uploaded by the content owner. 
| claimed | self | The row contains data for claimed content uploaded by the content owner. 
| claimed | thirdParty | The row contains data for claimed content uploaded by a third party. 