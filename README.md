# Automatic Inbox Cleanup with Two Simple Filters/Rules

<p align="center">
  <img width="380" height="429" src="https://github.com/Leftium/gmail-unimportant-mail-filters/assets/381217/f49a8e40-cd5a-4e2c-abf2-6e6097029e3a">
</p>
  





Last month I received 1,236 emails, but only 47 emails reached my inbox. These were the truly important emails I wanted to see, mostly sent from real people. These are the only emails that triggered a notification on my phone as soon as they hit my inbox.

The other 96% of the emails were silently and automatically filed into other categories/labels, without a single notification. About once a day, I take a few seconds to check them in bulk. I just scan the subjects and senders to mark a few bulk/automated emails that interest me. Then two keystrokes marks all of them as read. Ten, twenty, a hundred at a time!

How can you have your email sorted like this? You just have to add a few custom email filters/rules. Instructions and downloadable Gmail filter files are at the end of this article! 

## First, a Quick Tour of my Email Folders

Before explaining the email filters, it may help to understand the different categories my mail is sorted into. 

### Inbox Categories

I use [Gmail inbox categories & tabs](https://support.google.com/mail/answer/3094499?hl=en&visit_id=638344175390965025-3461488549&p=inboxtabs&rd=2), so my inbox is divided into three categories (Inbox categories & tabs helps a tiny bit, but the filters below do 99% of the work.):

1. **Primary:** those 47 truly important emails, and nothing else, end up here. If I star an email, that email also goes into Primary until unstarred.
2. **Updates:** Mostly automated emails informing me something happened, but usually don't require immediate attention.

|Sample Subject  | Sender |
|--|--|
|Your Savings statement is ready. | Apple Card \| Savings Support |
|Security alert | Google|
|Your Cloudflare Purchase Confirmation | Cloudflare |
|Successfully published userfront-svelte@0.0.2 | npm |

3. **Promotions:**  Mostly marketing emails, but some are more "updates" like HN Replies, Google Alerts, and vercel[bot].

|Sample Subject  | Sender |
|--|--|
| 👋 Act Fast - 20% Off Sitewide | iHerb |
| Price drop alert: $79.99 - Samsung 990 PRO Series | camelcamelcamel |
| Google Alert - meta quest | Google Alerts |
| [HN Replies] Re: How to Move Your Google Photos | HN Replies |
| Re: [Leftium/blues] Add more lead/follow text. (e6aaa59) | vercel[bot] |

### Tags/Folders

In addition, I have two tags:
- `sub` This email has 'unsubscribe' in the text. Most of these subscription emails are low priority. Usually filed into the "Promotions" category.
- `fyi` This email does not have 'unsubscribe' in the text, but it seems to have been sent via automated means. Usually filed into the "Updates" category.

The "Primary," "Updates," and "Promotions" Inbox categories are only available in Gmail, but all email services/clients should support the `sub` and `fyi` tags/folders.

### The two tags (and categories) are helpful when searching for email, too:
- To search just your important emails: exclude emails with `sub` and `fyi` tags.
- To search for an update email (like an order confirmation), search emails containing only `fyi` tags.
- Sometimes you may want to search through your marketing emails. If you're running out of Gmail storage, deleting emails with the `sub` tag is a great place to start!

## My Email Filters Explained

Email [filters](https://support.google.com/mail/answer/6579?hl=en) or [rules](https://www.hubspot.com/email-signature-generator/create-rules-outlook) are tiny programs that scan all your incoming mail and automatically take actions on them (like mark as read, move, or even delete them) if they meet certain conditions.

I created about two or three filters based on basic heuristics of what makes an email important or not.

### 1. The "Unsubscribe" filter

This simple rule singlehandedly does 80% of the work! If an email contains the word "unsubscribe," the email is probably not important. It's just not a common term used by most people. (Try searching your own email for ["unsubscribe"](https://mail.google.com/mail/u/0/#search/%22unsubscribe%22) right now!) But most marketing emails (in the US) are legally required to have an "unsubscribe" link. Thus most legitimate mass marketing emails include the word.

When an email contains "unsubscribe," this rule does two things:
1. Apply label `sub`
2. Categorize as "Promotions"

That's enough to keep 80-90% of uninteresting marketing emails from touching my inbox. Your mileage may vary. For example, this rule doesn't work in Korea. However Korean marketing emails must start the subject with the word "광고." So I made a similar filter for Korean emails (I actually combined the two filters into a single filter.)

### 2. The (Boring) Sender Filter(s)

Emails from "no-reply" are rarely interesting. It's a telltale sign the email was automatically sent. (Check for your own emails [sent from no-reply](https://mail.google.com/mail/u/0/#search/from%3Ano-reply).) However these emails tend to be less marketing and more informational. So I set up a different filter to catch these:

When an email is `from:noreply` *and does not contain "unsubscribe:"*
1. Appy label `fyi`
2. Categorize as "Updates"

There are actually many different boring senders besides  "no-reply."

- **Variations on "no-reply":** no.reply, noreply, do-not-reply, do_not_reply
- **Notifications:** notifications, notification, notify
- **Other boring senders:** webmaster, updates, tracking, support, postmaster, orders, info
- **Boring domains:** @amazon.com, @txt.voice.google.com, @googlecode.com, @emailonline.chase.com, @cc.yahoo-inc.com
- **Boring email addresses:** afund@umn.edu, linkedin@em.linkedin.com, 

There are so many variations, I actually had to split this rule into three different filters because it exceeded the maximum filter length. See my filters for the full list!

After setting up the "Unsubscribe" filter, I started examining the senders of the unimportant emails that still got through and added them to my boring senders filter until none got through.

### 3. The Vanguard Filter

Vanguard is very good at making their marketing emails look important. I had to create a special filter just for them:

If the email contains: "Because you're a valued Vanguard client, we thought you'd be interested in this information.":
1. Apply label `sub`
2. Categorize as "Promotions"

(Treated just like "unsubscribe" emails. These emails probably should have an "unsubscribe" link.)


## How to Set Up the Email Filters















