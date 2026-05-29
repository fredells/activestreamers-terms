# Terms of Service

**Last updated:** May 26, 2026

**Activestreamers** is a Reddit [Devvit](https://developers.reddit.com) app. By using it in a subreddit or viewing a post that uses it, you agree to these terms and to Reddit’s [User Agreement](https://www.reddit.com/policies/user-agreement) and [Content Policy](https://www.reddit.com/policies/content-policy).

Moderators choose the post title, Twitch category URL, and optional Steam store URL. Stream lists and prices come from Twitch and Steam and may be wrong or outdated. **Steam prices are informational only**—confirm on the store before buying. Twitch and Steam use is subject to their own terms. The app is provided **as is**, without warranties, to the extent allowed by law.

**Contact:** [message u/OttawaValley613 on Reddit](https://www.reddit.com/message/compose/?to=OttawaValley613)

# Privacy Policy

**Last updated:** May 26, 2026

This application stores configuration on each **custom post** when a subreddit moderator creates it, and fetches **public** game/stream/price data when someone opens the post.

**For each post, the app stores:**

- post title
- Twitch category URL (e.g. `twitch.tv/directory/category/…`)
- Steam store URL (optional — `store.steampowered.com/app/…`)

**When you view a post, the app also uses:**

- Reddit/Devvit post context (so it knows which post to load)
- your selected **Steam store region** from the in-post picker (country code such as `us`, `gb`; defaults to US)

**Caching:** API responses (stream lists and Steam prices) may be cached in Redis for about **one minute** to reduce load on Twitch and Steam. Cache entries contain public game data, not a profile of individual Reddit users.

**HTTP fetch — Twitch:** the app calls `id.twitch.tv` and `api.twitch.tv` using Twitch app credentials stored in **Devvit app settings** (not in post data). It requests public category/stream data for the Twitch URL on the post. No Reddit viewer account data is sent to Twitch.

**HTTP fetch — Steam:** when a Steam store URL is on the post, the app calls `store.steampowered.com` with the app id from that URL and the selected store region. It requests public store pricing (`appdetails`). No Reddit viewer account data is sent to Steam.

**What we do not do:** we do not sell personal information. We do not send Reddit passwords, emails, or Twitch/Steam logins to third parties.

For Reddit account or subreddit data, use Reddit’s [Privacy Policy](https://www.reddit.com/policies/privacy-policy).

**Contact:** [message u/OttawaValley613 on Reddit](https://www.reddit.com/message/compose/?to=OttawaValley613)
