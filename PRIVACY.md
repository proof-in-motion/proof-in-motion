# VidGen pipeline privacy policy

Effective October 29, 2026.

## Operator and purpose

VidGen pipeline is a private application operated by the owners of the [Proof in Motion channel](https://www.youtube.com/@proofinmotiontv). It is used for that channel's production, owner-approved uploads and internal reporting. It is not available for other creators to connect accounts.

The application uses **YouTube API Services**. Google's use of information is described in the [Google Privacy Policy](https://policies.google.com/privacy). Use of YouTube is also subject to the [YouTube Terms of Service](https://www.youtube.com/t/terms).

## Information accessed and stored

Google handles OAuth sign-in and consent. VidGen does not request or store Google passwords. It stores the channel owner's OAuth access and refresh tokens in a private token file so authorized tasks can run without repeated sign-in. The requested permissions allow uploading videos, reading channel information and reading the owner's channel analytics, including estimated revenue when available.

The application stores uploaded video identifiers and operational logs, owner-created titles, descriptions, thumbnails and video files, and the owner's aggregate daily channel metrics: views, watch time, average view duration, subscribers gained and estimated revenue. A private SQLite database and generated monthly reports support the owners' production records and expense settlement. VidGen does not retrieve individual viewers' identities, contacts, private messages or browsing history.

Competitor-metric research is disabled in the audit configuration. Enabling that feature requires approval of its use case and derived metrics, and an updated disclosure before use. It is not needed to publish the channel's videos.

## Use and sharing

Finished media and approved metadata are sent to YouTube for upload. YouTube applies the selected privacy setting and its own platform restrictions. Channel analytics and tokens are available only to the owners and the agents they authorize to administer this installation. They are not sold, used for targeted advertising, or supplied as inputs to external research services.

Production services may receive owner-created scripts, images and audio to produce the channel's media. They do not need the owner's YouTube OAuth tokens or private analytics. The operator must keep credentials and analytics out of production prompts, public repositories, demonstrations and support attachments.

The command-line application has no embedded advertising player, browser cookies, or advertising trackers. This documentation is hosted by GitHub, whose handling of visitors' data is covered by the [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Security and retention

Tokens are stored in files restricted to the operating-system account that runs VidGen; secrets are excluded from source control and public documentation. Operators must similarly restrict access to the database, reports and backups.

Tokens and owner-authorized Analytics API data are retained only while needed for the disclosed purpose and while authorization remains valid. The scheduled analytics sync checks authorization with Google. Operators must keep this check running at least once every 30 days, verify stored uploads have not been deleted, and remove data that is no longer authorized. Temporary service failures are not treated as revocation.

There is no permanent cache of other channels' API metadata in the audit configuration. Original production files and expense amounts are the owners' records and are separate from data retrieved from YouTube.

## Revocation and deletion

An owner can revoke access at any time using [Google Account permissions](https://myaccount.google.com/permissions). The installed client also provides `vidgen auth disconnect-youtube`, which requests revocation from Google and clears that installation's token, stored channel analytics, upload identifiers and generated monthly reports. If Google reports that authorization is no longer valid during the scheduled check, the installation clears its local YouTube data.

An owner may also request deletion through the operator contact below. The operator must process deletion requests and removal after in-app revocation as soon as possible and within **seven days**, including copies in other installations, exports and backups. Revocation through Google settings must be detected and acted on within **30 days**. Backup copies must follow the same deletion requirements; deleting one installation does not erase other copies automatically.

Removing data from VidGen does **not** delete videos or other information stored by YouTube. Use YouTube Studio to manage or delete those videos. Original production media and expense amounts can remain after disconnection; they do not authorize further access to YouTube.

## Contact and changes

Contact the operator through [the channel's documentation support form](https://github.com/vidgen-studio/channel-info/issues/new). This is a public issue form: do not include tokens, private analytics, mailing addresses or other sensitive data. The operator can arrange a private follow-up for an identity-verified owner.

Changes to the data accessed, shared or used require an updated policy and renewed owner consent before the changed processing begins. The effective date above identifies this version.
