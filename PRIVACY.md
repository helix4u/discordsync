# DiscordSync privacy policy

Last updated: October 2, 2026.

## Operator and purpose

DiscordSync is operated by helix4u as a personal helper for support work. It copies
relevant public Discord support-thread information into a local troubleshooting
workspace. The operator uses it to investigate reported problems, follow up on
unresolved questions, and maintain support records and reports.

## Information processed

DiscordSync processes the messages, titles, displayed author names, Discord user
and message identifiers, timestamps, thread status, and attachments supplied in
the configured public support threads. Public visibility does not mean that the
copied records are anonymous. The helper does not require user-presence data or
a complete server-member list.

The copied archive is for the operator's support work. It is not published through
this repository or sold as a dataset.

## AI-assisted troubleshooting

The operator uses relevant support material with Hermes and ChatGPT to help
troubleshoot issues and prepare support responses. Provider training on submitted
data is disabled for this workflow. Provider-side storage and deletion depend on
the applicable service settings and terms. Disabling training does not imply that
a provider retains no data. The operator does not use the archive to train models.

## Retention

DiscordSync's conversation archive and generated case caches use a rolling
30-day retention limit for raw message content.
Downloaded attachments use a rolling 14-day limit. Age is measured from the
original Discord message timestamp, including for open support cases.

Cleanup runs during synchronization and through hourly local housekeeping while
the operator's Windows account is signed in. Missed housekeeping resumes at
sign-in. Expired content is excluded from subsequent synchronization and backfill.
Generated local case caches follow the same content limits.

Minimal case dates, status, counts, and identifiers can remain when needed for
support reporting or to prevent removed content from being copied back. They
are removed when no longer needed or when an applicable deletion request requires
it. Generalized troubleshooting findings can be retained after identifying
details have been removed.

Recovery snapshots contain case metadata, without raw conversation bodies or
downloaded attachments. Earlier full-data snapshots are replaced with verified
metadata-only copies. Restoring an archive must preserve current deletion and
retention records. These snapshots are not published in this repository.

## Correction and deletion requests

If your thread has been handled using this helper, ask the operator directly in
the support conversation to correct or delete copies held from it. If that thread
is closed, raise a new support thread referring to the original conversation.
No separate DiscordSync account is required.

The operator verifies the request against the relevant Discord identity and thread
and handles it promptly. This includes relevant local transcripts, attachments,
indexes, copied reports, exports, backups, and affected AI-service conversations
under the operator's control. A successful local cleanup is not treated as proof
that every downstream copy has been removed.

Deleting copied records does not delete the original messages on Discord.

## Protection and contact

Access to copied support records is restricted to the operator's support
workflow. The working archive, generated case caches, and recovery snapshots are
encrypted at rest. DiscordSync uses HTTPS when retrieving information from Discord.

Questions, correction requests, deletion requests, or concerns about DiscordSync
can be raised with helix4u through the support conversation in which the helper
was used.
