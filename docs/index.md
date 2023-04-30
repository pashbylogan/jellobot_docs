# Welcome to Jellobot

This is a discord bot whos purpose is to support Dawn of Arawn in its administrative duties for the
game [Celtic Heroes](https://celtic-heroes.com/).

## Features

- Tracks dl/edl attends and endgame
- Calculates kp, DG, seed, and all other points on a monthly or "all time" basis
    - Including the ranking commands (e.g. "top")
- Track which drops have been bought by players
    - Subtracts points when bids are completed
- Spam when bosses are due
- Boss queue management
    - amend - Change the time or name of a boss entry in the queue
    - pop - Remove an entry from the queue
    - push - Add an entry to the queue
    - queue - Print the queue

## How does it work?
Jellobot is a Discord bot designed to assist with administrative tasks for the game Celtic Heroes. It is built using the [Discord.py](https://discordpy.readthedocs.io/en/stable/index.html) library and uses a Postgres database to store user data, points, timers, and other relevant information.

When Jellobot is added to a Discord server, it can be used by server members to track their attendance at dl/edl raids and earn points for attending. The bot can also track other events and calculate points on a monthly or "all time" basis. The points earned by users can be used to bid on drops, which Jellobot also tracks.

In addition to tracking attendance and drops, Jellobot can also send reminders when bosses are due and manage a boss queue. Users can add, remove, or modify boss entries in the queue using simple commands.

All data required for Jellobot's functionality is stored in a Postgres database. When a user attends a raid or bids on a drop, Jellobot updates the relevant data in the database. When a boss reminder is due or a boss queue command is executed, Jellobot retrieves the relevant data from the database and executes the required action. Before, the discord bot was using google sheets for it's data store. That definitely had it's advantages, but at some point the amount of cells got to a point where a bona fide database would work better. Speeds drastically improved from this change at the cost of user visibility.

Jellobot's code is modular and easy to understand, making it easy for developers to add new features or modify existing ones. The bot's author, @pashbylogan, is always happy to receive feedback and suggestions for new features.

## Asynchronous Programming
Jellobot uses asynchronous programming techniques to improve performance and responsiveness. Asynchronous programming allows Jellobot to handle multiple tasks simultaneously, without blocking the execution of other code. In python, this is generally done with the asyncio library.

In addition to using asyncio, Jellobot also uses the asyncpg library for database access. asyncpg is an asynchronous PostgreSQL database client library that is designed to work with asyncio. Switching from psycopg2 to asyncpg improves Jellobot's performance by allowing it to handle multiple database queries concurrently.

With asyncpg, Jellobot can execute multiple database queries simultaneously, without blocking the execution of other code. This allows Jellobot to handle high loads of incoming requests and execute multiple queries concurrently, resulting in faster response times and improved performance.


## Environment Variables

To run this project, you will need to add the following environment variables to your .env file

`DATABASE_URL` - The connection string for a Postgres database containing all data that the app relies on.

`DISCORD_TOKEN` - Determines which discord bot is actually run with the functionality described in the code. This bot
will have to be added to any server you want to use it on.
See [adding a discord bot to a server](https://www.howtogeek.com/744801/how-to-add-a-bot-to-discord/) for more
information.

## Deployment

To deploy this project run

```bash
  python wsgi.py
```

## FAQ

#### Can I use this for my own clan?

Yes, but you may have to make some modifications to fit your personal use case. Please reach out if you are going to use
my code for your own purposes.

#### Can you add a new feature or make edits to how it currently works?

Definitely, but I built this in my free time to help Dawn. Major updates may take me time to plan and implement so
please bear with me.

## Authors

- [@pashbylogan](https://www.github.com/pashbylogan)

## Feedback

If you have any feedback, please reach out to us at pashbylogan@gmail.com.
