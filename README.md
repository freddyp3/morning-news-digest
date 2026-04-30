# Morning News Digest

Local n8n workflow that sends a morning email digest with:

- Chelsea news
- Daily to-dos
- Tech news
- Nintendo most-read news

## Notes

- If you want to try it out you have to add your own credentials.
- Update the file path in the "Read/Write Files from Disk" node to point to your local `watchlist.csv`.

## To Run

1. Create your .env
2. Start n8n with env loaded:

    - ```bash export N8N_BLOCK_ENV_ACCESS_IN_NODE=false```
    - ```bash source .env ```
    - ```bash n8n```

3. import the workflow
