# ![LOGO](logo.png) iQualify **flow**ground Connector

## Description

A generated **flow**ground connector for the iQualify API (version v1).

Generated from: https://api.apis.guru/v2/specs/iqualify.com/v1/swagger.json<br/>
Generated at: 2019-05-07T17:42:29+03:00

## API Description

The iQualify API offers management and analytics responses for building
learning experiences using your iQualify instance data.

Once you’ve registered with iQualify, you can request an API access token by
navigating to the API access section of the "Account Settings" area.

Find out how to [Request your API access token](https://intercom.help/iqualify/iqualify-set-up/authentication/requesting-your-api-access-token) on our Knowledge base.

All endpoints are only accessible via https and are located at
api.iqualify.com. For instance: you can find your current offerings by
accessing the following URL:

    https://api.iqualify.com/v1/offerings/current



## Authorization

Supported authorization schemes:
- API Key
## Actions

### List supported endpoints URLs

> Responds with all supported endpoints URLs for v1 version.

*Tags:* `API info`

### Find course mappings

> Returns all the course mappings

*Tags:* `course mappings`

### Finds course mappings by offering id

*Tags:* `course mappings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Remove course mapping

> Removes the course mapping between the offering and the external course id

*Tags:* `course mappings`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `externalCourseId` - _required_ - external course's id

### Add course mapping

> Creates a mapping between the offering and the external course id

*Tags:* `course mappings`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `externalCourseId` - _required_ - external course's id

### Find courses

> Responds with courses that can be activated (made to an offering).

*Tags:* `courses`

### Find course by content id

*Tags:* `courses`

#### Input Parameters
* `contentId` - _required_ - The content Id

### Update course category

*Tags:* `courses`

#### Input Parameters
* `contentId` - _required_ - The content Id

### Update course level

*Tags:* `courses`

#### Input Parameters
* `contentId` - _required_ - The content Id

### Update course tags

*Tags:* `courses`

#### Input Parameters
* `contentId` - _required_ - The content Id

### Update course topic

*Tags:* `courses`

#### Input Parameters
* `contentId` - _required_ - The content Id

### Update course access

*Tags:* `courses`

#### Input Parameters
* `contentId` - _required_ - The content Id

### Get current, past and future offerings

> Responds with all offerings for your organisation.

*Tags:* `offerings`

### Create offering

> Creates new offering.

*Tags:* `offerings`

### Find active offerings

> Responds with current (active) offerings for your organisation. Offering is current when today's date is between (inclusive) it's `start` and `end` date.

*Tags:* `offerings`

### Find future offerings

> Responds with future (inactive) offerings for your organisation. Future offerings have their `start` date after today's date (inclusive).

*Tags:* `offerings`

### Find past offerings

> Responds with past (inactive) offerings for your organisation. Past offerings have their `end` date before today's date (inclusive).

*Tags:* `offerings`

### Find offering by id

> Returns an offering matching the offeringId.

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Update offering

> Updates the offering.

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find comments

> Responds with a list of all comments in any of the posts for a channel in a offering

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `channelId` - _required_ - channel's id

### Find posts

> Responds with a list of posts for a channel in a offering

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `channelId` - _required_ - channel's id

### Find replies

> Responds with a list of all replies in any of the posts for a channel in a offering

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `channelId` - _required_ - channel's id

### Find learners progress

> Responds with learners progress.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find assignments marks

> Responds with assignments marks.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find quizzes marks

> Responds with quizzes marks.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find pulses ids

> Returns ids of all pulses that learners responded to.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find pulses by offeringId

> Returns pulses' responses matching the offeringId.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `pulseType` - _optional_ - Filter pulse responses by type.
    Possible values: submit_text, MCQ, spatial_triangular, spatial_planar, spatial_linear.
* `responseTime` - _optional_ - Filter pulse responses by responseTime. Lower then (`lt`), lower then or equal (`lte`), greater then (`gt`) and greater then or equal (`gte`) operators are available. Example of filtering by time range __responseTime=gte\_\_2017-03-14T07:30:00Z&responseTime=lte\_\_2017-03-16T09:30:00Z__

### Find pulses by offeringId and pulseId

> Returns pulse's responses matching the offeringId and pulseId.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `pulseId` - _required_ - pulse's base id

### Find submissions to assignments, including marks if any

> Responds with assignments submissions.

*Tags:* `analytics`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find offering's assessments

> Get all offering's assessments

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Update assessment details

> Modifies assessment details

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `assessmentId` - _required_ - assessment's id

### Upload new document

> Uploads assessment document file

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `assessmentId` - _required_ - assessment's id

### Remove the document

> Removes assessment document file

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `assessmentId` - _required_ - assessment's id
* `documentId` - _required_ - documents's id

### Find channels

> Responds with a list of channels in a offering

*Tags:* `channels`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Add channel

> Adds new channel to the offering

*Tags:* `channels`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Update channel

> Updates the channel

*Tags:* `channels`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `channelId` - _required_ - channel's id

### Set offering's cover image

> Replaces offering's cover image with uploaded image

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find assessment groups

> Responds with a list of assessment groups in an offering

*Tags:* `assessment groups`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Add an assessment group

> Creates a new assessment group in a offering

*Tags:* `assessment groups`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find learners in an assessment group

> Responds with a list of learners for the assessment group

*Tags:* `assessment groups`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `groupId` - _required_ - Assessment group id

### Add a learner to an assessment group

*Tags:* `assessment groups`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `groupId` - _required_ - Assessment group id

### Remove a learner from an assessment group

*Tags:* `assessment groups`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `groupId` - _required_ - Assessment group id
* `userEmail` - _required_ - user's email

### Update offering category metadata

> Updates the offering category metadata.

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Update offering level metadata

> Updates the offering level metadata.

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Update offering tags metadata

> Updates the offering tags metadata.

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Update offering topic metadata

> Updates the offering topic metadata.

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Set offering's study plan

> Replaces offering's study plan with uploaded file

*Tags:* `offerings`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Find offering's users

> Responds with a list of offering's users (facilitators, learners and markers).

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `facilitators` - _optional_ - If true, facilitators are included in the results.
* `learners` - _optional_ - If true, learners are included in the results.
* `markers` - _optional_ - If true, markers are included in the results.

### Adds user to the offering.

> Adds one or more users to the offering.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id

### Remove learners from evaluator's list.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `evaluatorEmail` - _required_ - evaluator's id

### Find learners evaluated by the peer evaluator.

> Get learners evaluated by the peer evaluator.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `evaluatorEmail` - _required_ - evaluators's email

### Add learners to be evaluated by the peer evaluator.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `evaluatorEmail` - _required_ - evaluator's email

### Remove learners from marker's list.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `markerEmail` - _required_ - marker's email

### Find Learners marked by the marker.

> Get learners marked by the marker.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `markerEmail` - _required_ - marker's email

### Add learners to be marked by the marker.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `markerEmail` - _required_ - marker's email

### Removes user from the offering.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `userEmail` - _required_ - user's email

### Re-sends the invitation e-mail.

> Re-sends the invitation e-mail to the user.

*Tags:* `offering users`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `userEmail` - _required_ - user's email

### Gets user's open response assignment submissions

> Gets user's open response assignment submissions.

*Tags:* `submissions`

#### Input Parameters
* `offeringId` - _required_ - offering's id
* `userEmail` - _required_ - user's email

### Add new user

> Adds new user

*Tags:* `users`

### Learner progress for all offerings

> Returns offering progress for each learner

*Tags:* `analytics`

#### Input Parameters
* `$top` - _optional_ - Returns only the first n results.
* `$orderby` - _optional_ - Sorts the results.
* `$filter` - _optional_ - Filters the results, based on a Boolean condition.

### Find user by email

> Returns a user matching the email.

*Tags:* `users`

#### Input Parameters
* `userEmail` - _required_ - user's email

### Update the user

> Updates the user

*Tags:* `users`

#### Input Parameters
* `userEmail` - _required_ - user's email

### Get user's offerings

> Responds with all user's offerings.

*Tags:* `users`

#### Input Parameters
* `userEmail` - _required_ - user's email

### Add permission to user

> Adds permission to user

*Tags:* `users`

#### Input Parameters
* `userEmail` - _required_ - user's email
* `permissionName` - _required_ - permission name
    Possible values: builder, manager.

## License

**flow**ground :- Telekom iPaaS / iqualify-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
