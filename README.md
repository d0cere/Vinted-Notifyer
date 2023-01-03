<h1 align="center">
    <img src="https://cdn.discordapp.com/attachments/1053742552009941075/1059788849087266897/banner.png" alt="mftool-java">
  </a>
</h1>


# Vinted Notifyer
This is a web application written in Flask that allows users to set up email notifications for new items on Vinted that match certain criteria (e.g. specific brand, price range, etc.).

## Features
- Set up email notifications for new items on Vinted that match certain criteria.
- View a history of past search queries and email notifications.
- Modify or delete existing search queries.
- Set price filters for certain items.

## Source
At present, the Vinted Notifier is not open source nor is it accessible to the general public. This is due to my inconsistent schedule and lack of availability to work on the project. In the future, I hope to commercialise the Vinted Notifier and make it readibly available to the public. However, at this time, I do not believe that it would be a viable option.

## How it works
The Vinted Notifier operates by storing all items that the user has specified in an SQL database. At irregular intervals (in order to avoid rate limits), the bot will make a request to the specified URL and scrape the newest items. The unique IDs of these items are then recorded in the database, ensuring that the same item is not emailed to the user multiple times.
