# Automatic Inbox Cleanup with Two Simple Filters/Rules

<p align="center">
  <img width="380" height="429" src="https://github.com/Leftium/gmail-unimportant-mail-filters/assets/381217/f49a8e40-cd5a-4e2c-abf2-6e6097029e3a">
</p>


Last month I received 1,236 emails, but only 47 emails reached my inbox. These were the truly important emails I wanted to see, mostly sent from real people. These are the only emails that triggered a notification on my phone as soon as they hit my inbox.

The other 96% of the emails were silently and automatically filed into other categories/labels without a single notification. About once a day, I take a few seconds to check them in bulk. I just scan the subjects and senders to mark a few bulk/automated emails that interest me. Then two keystrokes marks all of them as read. Ten, twenty, a hundred at a time!

How can you have your email sorted like this? You just have to add a few custom email filters/rules. Instructions and downloadable Gmail filter files are at the end of this article! 

## TL;DR (Quick Instructions)

 - Instructions for Gmail web app; read the detailed explanation for other services/clients.
 - Use one of the methods below (no need to do both):

### Gmail Filter/Search Links

Follow the links, click "Create Filter", then finish wizard.

1. [Unsubscribe][filter-unsubscribe]
2. [Boring Sender Part I][filter-boring-sender-1]
    - [Boring Sender Part II][filter-boring-sender-2]
    - [Boring Sender Part II][filter-boring-sender-3]
3. [Vanguard][filter-vanguard]

### Gmail Filter XML Exports

Download raw files, go to [Gmail Settings > Filters](https://mail.google.com/mail/u/0/#settings/filters), then click "Import filters".

1. [Unsubscribe Filter.xml](https://github.com/Leftium/gmail-unimportant-mail-filters/blob/main/1.%20Gmail%20Unsubscribe%20Filter.xml)
2. [Boring Sender Filter.xml](https://github.com/Leftium/gmail-unimportant-mail-filters/blob/main/2.%20Gmail%20Boring%20Sender%20Filter.xml)
3. [Vanguard Filter.xml](https://github.com/Leftium/gmail-unimportant-mail-filters/blob/main/3.%20Gmail%20Vanguard%20Filter.xml)


[filter-unsubscribe]: https://mail.google.com/mail/u/0/#create-filter/has=%7B+unsubscribe+subject%3A%EA%B4%91%EA%B3%A0++%7D&sizeoperator=s_sl&sizeunit=s_smb
[filter-boring-sender-1]: https://mail.google.com/mail/u/0/#create-filter/from=naverpayadmin_noreply%7C+success%7C+onlinemart%7C+itinerary%7C+anaintrsv%7C+vessifootwear%7C+cm.bsaefiling%7C+noreply_us%7C+ownerverification%7C+onboarding%7C+Specialrisk%7C+Confirmation%7C+policies%7C+custsrv%7C+notifs%7C+team%7C+admin%7C+theplan%7C+customercscenter%7C+marketing%7C+alerts%7C+billing_info%7C+billpay%7C+communications%7C+customer_service%7C+do-not-reply%7C+do_not_reply%7C+emsnts%7C+info%7C+newsletter%7C+news%7C+no-reply%7C+no.reply%7C+noreply%7C+notifications%7C+notification%7C+notify%7C+orders%7C+postmaster%7C+support%7C+tracking%7C+updates%7C+webmaster&hasnot=%7B+unsubscribe+subject%3A%EA%B4%91%EA%B3%A0+%7D&sizeoperator=s_sl&sizeunit=s_smb
[filter-boring-sender-2]: https://mail.google.com/mail/u/0/#create-filter/from=%40emailonline.chase.com%7C+robin_j%40naver.com%7C+j_ote%40hackerx.co%7C+%40cc.yahoo-inc.com%7C+%40chrometa.com%7C+%40dreamhost.com%7C+%40googlecode.com%7C+%40livejournal.com%7C+%40perception-point.io%7C+%40seoulplayers.com%7C+afund%40umn.edu%7C+cs%40umn.edu%7C+i-jkwon%40microsoft.com%7C+linkedin%40em.linkedin.com%7C+pwexpire%40umn.edu%7C+umatters%40umn.edu%7C+bounce%2Bsignup%40fastmail.fm&hasnot=%7B+unsubscribe+subject%3A%EA%B4%91%EA%B3%A0++%7D&sizeoperator=s_sl&sizeunit=s_smb
[filter-boring-sender-3]: https://mail.google.com/mail/u/0/#create-filter/from=%40firstpay.co.kr%7C+%40fiserv.com%7C+%40messaging.squareup.com%7C+%40splunk.com%7C+%40comfycomfy.com%7C+brian%40dancemardigras.com%7C+%40lpoint.com%7C+%40pinggy.io%7C+%40hanssem.com%7C+%40codesandbox.io%7C+%40order.dell.com%7C+hello%40earthrunners.com%7C+store%40shopblenheimgingerale.com%7C+tilley%40tilley.com%7C+%40accts.epicgames.com%7C+%40amazon.com%7C+%40asktheheadhunter.com%7C+%40auction.co.kr%7C+%40banking.salliemae.com%7C+%40biberk.com%7C+%40bluevirtual.com%7C+%40clientexperience.citi.com%7C+%40crm.interpark.com%7C+%40e-mail.microsoft.com%7C+%40ealerts.bankofamerica.com%7C+%40ebay.com%7C+%40fiscal.treasury.gov%7C+%40godaddy.com%7C+%40googlegroups.com%7C+%40googlemail.com%7C+%40investordelivery.com%7C+%40lists.sourceforge.net%7C+%40mail.sp.sofi.com%7C+%40mvno.kt-bill.kt.com%7C+%40notification.capitalone.com%7C+%40o.sofi.org%7C+%40paypal.com%7C+%40txt.voice.google.com%7C+%40ups.com%7C+%40welcome.americanexpress.com%7C+aloha%40shortwave.com%7C+ant%40supabase.io%7C+appleid%40id.apple.com%7C+citibank.message%40%7C+contact%40executeprogram.com%7C+csealumni%40umn.edu%7C+feedback%40minaal.com%7C+spark%40readdle.com%7C+venmo%40venmo.com%7C+waitlist%40isthereanydeal.com&hasnot=%7B+unsubscribe+subject%3A%EA%B4%91%EA%B3%A0++%7D&sizeoperator=s_sl&sizeunit=s_smb
[filter-vanguard]: https://mail.google.com/mail/u/0/#create-filter/has=%22Because+you're+a+valued+Vanguard+client%2C+we+thought+you'd+be+interested+in+this+information.%22&sizeoperator=s_sl&sizeunit=s_smb 

## Detailed Explanation/Instructions

### First, a Quick Tour of my Email Folders

Before explaining the email filters, it may help to understand the different categories my mail is sorted into. 

#### Inbox Categories

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

#### Tags/Folders

In addition, I have two tags:
- `sub` This email has 'unsubscribe' in the text. Most of these subscription emails are low priority. Usually filed into the "Promotions" category.
- `fyi` This email does not have 'unsubscribe' in the text, but it seems to have been sent via automated means. Usually filed into the "Updates" category.

The "Primary," "Updates," and "Promotions" Inbox categories are only available in Gmail, but all email services/clients should support the `sub` and `fyi` tags/folders.

#### The two tags (and categories) are helpful when searching for email, too:
- To search just your important emails: exclude emails with `sub` and `fyi` tags.
- To search for an update email (like an order confirmation), search emails containing only `fyi` tags.
- Sometimes you may want to search through your marketing emails. If you're running out of Gmail storage, deleting emails with the `sub` tag is a great place to start!

### My Email Filters Explained

Email [filters](https://support.google.com/mail/answer/6579?hl=en) or [rules](https://www.hubspot.com/email-signature-generator/create-rules-outlook) are tiny programs that scan all your incoming mail and automatically take actions on them (like mark as read, move, or even delete them) if they meet certain conditions.

I created about two or three filters based on basic heuristics of what makes an email important or not.

#### 1. The "Unsubscribe" filter

This simple rule singlehandedly does 80% of the work! If an email contains the word "unsubscribe," the email is probably not important. It's just not a common term used by most people. (Try searching your own email for ["unsubscribe"](https://mail.google.com/mail/u/0/#search/%22unsubscribe%22) right now!) But most marketing emails (in the US) are legally required to have an "unsubscribe" link. Thus most legitimate mass marketing emails include the word.

When an email contains "unsubscribe," this rule does two things:
1. Apply label `sub`
2. Categorize as "Promotions"

That's enough to keep 80-90% of uninteresting marketing emails from touching my inbox. Your mileage may vary. For example, this rule doesn't work in Korea. However Korean marketing emails must start the subject with the word "광고." So I made a similar filter for Korean emails (I actually combined the two filters into a single filter.)

#### 2. The (Boring) Sender Filter(s)

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

#### 3. The Vanguard Filter

Vanguard is very good at making their marketing emails look important. I had to create a special filter just for them:

If the email contains: "Because you're a valued Vanguard client, we thought you'd be interested in this information.":
1. Apply label `sub`
2. Categorize as "Promotions"

(Treated just like "unsubscribe" emails. These emails probably should have an "unsubscribe" link.)


## How to Set Up the Email Filters (Detailed Version)

Coming soon...

















