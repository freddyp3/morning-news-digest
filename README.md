# Morning News Digest

Local n8n workflow that sends a morning email digest with:

- Chelsea news (reddit)
- Daily to-dos (notion)
- Tech news (hackerNews)
- Nintendo most-read news
- Stock watchlist (via TwelveData API)

## Setup Req

### Setup own credentials

- SMTP (sending emails)
- Notion API (for To-Do integration)
- TwelveData API key (put this in a .env file with variable name TWELVE_DATA_API_KEY)
  
### Other things

- Update the file path in the "Read/Write Files from Disk" node to point to your local `watchlist.csv`.
- Input your own email

## To Run

1. Create your .env
2. Start n8n with env loaded:

    - ```export N8N_BLOCK_ENV_ACCESS_IN_NODE=false```
    - ```source .env ```
    - ```n8n```

3. import the workflow
4. activate it

## Notes

- The workflow will only run automatically if n8n is running

## For the future

- Deploy to the cloud or run it on a Raspberry Pi for 24/7 automation
- Run news filtering through Ollama (Llama) on a Raspberry Pi (24/7 local inference)
- Preferred to get Nintendo news weekly, make it so we store each day, then use Ollama to sort the best 3.
- Add WhatsApp/Telegram integration to update stock watchlist dynamically.
- Incorporate Hacker News points into ranking logic
- Nicer looking final output
