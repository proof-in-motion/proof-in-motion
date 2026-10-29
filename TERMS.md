# Proof in Motion Studio terms of use

Effective October 29, 2026.

Proof in Motion Studio is a private command-line application for the owners of Proof in Motion and their authorized operators. It is not offered as a public upload service. Use requires the owners' permission and acceptance of the [privacy policy](PRIVACY.md).

The application uses YouTube API Services. **By using Proof in Motion Studio, you agree to be bound by the [YouTube Terms of Service](https://www.youtube.com/t/terms).** Operators must also comply with the [YouTube API Services Terms of Service](https://developers.google.com/youtube/terms/api-services-terms-of-service), [Developer Policies](https://developers.google.com/youtube/terms/developer-policies) and applicable YouTube content rules.

Only upload content the owners have the rights to use. An owner must review the media and its title, description, audience designation and visibility before authorizing publication. Operators can inspect the exact metadata using `vidgen publish VIDEO_ID --dry-run`; the source metadata and configuration remain editable by the owners. Additional language settings and YouTube features can be managed in [YouTube Studio](https://studio.youtube.com/).

API uploads from an unaudited project can be locked private by YouTube. Proof in Motion Studio cannot remove that restriction or guarantee approval of an audit. For public release while an audit is pending, follow Google's documented process of uploading through YouTube Studio. Do not misrepresent the audit status or switch projects to evade restrictions.

Operators must keep credentials private, preserve a human approval step, follow the privacy policy's deletion requirements and stay within both the channel's spending budget and Google's API quotas. Disconnect access through `vidgen auth disconnect-youtube` or [Google Account permissions](https://myaccount.google.com/permissions).

There are no subscription fees for this internal client. Production services may incur separately authorized expenses. The application is provided as available; availability, views, revenue and Google approval are not guaranteed. YouTube and Google are independent service providers and do not endorse Proof in Motion Studio or Proof in Motion.

Questions: [contact the operator](https://github.com/proof-in-motion/proof-in-motion/issues/new). Do not publish sensitive information in public issues.
