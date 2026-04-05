# Haven Intent Engine

A read-only Reddit research script that monitors public cryptocurrency security discussions across relevant subreddits using the Reddit OAuth2 Search API.

## What This Script Does

This tool searches public Reddit communities for posts and threads where users are discussing cryptocurrency security concerns, wallet safety, exchange risks, and custody solutions. The purpose is to understand the most common points of concern, confusion, and vulnerability that everyday crypto users are experiencing — identifying knowledge gaps and recurring questions within these communities.

## How It Works

- Connects to the Reddit Search API using standard OAuth2 script credentials
- Submits keyword-based search queries across specified public subreddits
- Reads post titles, body text, scores, and comment counts from public feeds
- Feeds results into an external scoring interface for categorisation and analysis
- Runs on a defined schedule within Reddit's standard rate limits

## Subreddits Monitored

- r/CryptoCurrency
- r/Bitcoin
- r/ethfinance
- r/defi
- r/CryptoSecurity
- r/ledgerwallet
- r/trezor
- r/cryptowallets
- r/selfhosted

## Data Handling

- Accesses public content only — no private messages, no restricted communities
- Does not store usernames or any personally identifiable information
- Does not store, sell, or share user data with any third party
- Reads only what is publicly visible to any Reddit visitor without an account

## What This Script Does NOT Do

- Does not post, comment, reply, or vote
- Does not interact with any Reddit user in any way
- Does not scrape beyond standard API rate limits
- Does not access any non-public content
- Does not collect or store personal data

## API Usage

- Authentication: OAuth2 script credentials
- Endpoints used: Reddit Search API (`/search`), public subreddit feeds
- Rate limiting: Fully compliant with Reddit's API terms — maximum 60 requests per minute
- User agent: Identifies correctly as per Reddit API guidelines

## Tech Stack

- Runtime: Node.js
- Auth: OAuth2 via Reddit script credentials
- External: Anthropic Claude API for post scoring and categorisation (read-only input)

## Compliance

This script is built in full compliance with Reddit's API Terms of Service and Developer Agreement. It operates as a passive research tool only, with no user interaction or data collection of any kind.
