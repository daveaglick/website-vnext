Title: COVIDSafe application TempID identifier was static
ReportedAt: 2020/04/27
ResolvedAt: 2020/05/14
Status: Resolved
---

# Overview

> The lifetime of this ID is important because it will uniquely identify your phone for this time interval. It doesn't say who you are, but it allows any Bluetooth device in range to know that it's the same phone it saw earlier. A simple example of how this could be abused is that it allows someone to track your movement as your ID shows up in multiple locations. Devices recording these IDs could provide effective distributed location tracing. This is why it's very important that the same ID is used for the shortest possible period.
> 
> A slightly more complicated example is that if I already know who someone is and can record their ID (by being within 20 metres of them for a few seconds), then I now can track that exact person. This would be especially worrying to victims of domestic violence (also note that the issues described here do not require access to an unlocked phone).

From: https://docs.google.com/document/d/1u5a5ersKBH6eG362atALrzuXo3zuZ70qrGomWVEC27U/edit#

<?# Twitter 1261109574263730177 /?>

# Timeline

- This issue was first reported to privacy@health.gov.au at 1:19am on 27/04/2020, and subsequently by in-app feedback later that day. It was also reported to asd.assist@defence.gov.au at 4:52pm on 27/04/2020.
- This issue was first reported to the Singapore OpenTrace team at 12:38am on 30/04/2020 and [was fixed in this commit](https://github.com/opentrace-community/opentrace-android/commit/0c7f7f6c4b265140f86b91f8e9e1ec70f5cd67ba) to the opentrace-android repository at 7:11pm on the same day.
- This issue was fixed in v1.0.17 released on 14/05/2020 (see note at end)