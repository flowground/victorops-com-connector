# ![LOGO](logo.png) VictorOps **flow**ground Connector

## Description

A generated **flow**ground connector for the VictorOps API (version 0.0.3).

Generated from: https://api.apis.guru/v2/specs/victorops.com/0.0.3/swagger.json<br/>
Generated at: 2019-05-07T17:44:37+03:00

## API Description

This API allows you to interact with the VictorOps platform in various ways. Your account may be limited
to a total number of API calls per month. Also, some of these API calls have rate limits.

NOTE: In this documentation when creating a sample curl request (clicking the TRY IT OUT! button), in some API
viewing interfaces, the '@' in an email address may be encoded. Please note that the REST endpoints will not
process the encoded version. Make sure that the encoded character '%40' is changed to its unencoded form before
submitting the curl request.


## Authorization

This API does not require authorization.

## Actions

### Retrieve alert details.

> Retrieve the details of an alert that was sent VictorOps by you.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Alerts`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `uuid` - _required_ - The VictorOps uuid of the alert

### Get current incident information

> Get a list of the currently open, acknowledged and recently resolved incidents.<br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Create a new incident

> Create a new incident.<br/>
> <br/>
> This call replicates the function of our<br/>
> <a href="https://help.victorops.com/knowledge-base/manual-incident-creation/">manual incident creation process</a>.<br/>
> Monitoring tools and custom integrations<br/>
> should be configured using our<br/>
> <a href="https://help.victorops.com/knowledge-base/victorops-restendpoint-integration/">REST Endpoint</a>.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Acknowledge an incident or list of incidents

> The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Acknowledge all incidents for which a user was paged.

> The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Resolve all incidents for which a user was paged.

> The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Reroute one or more incidents to one or more new routable destinations.

> Reroute one or more incidents to one or more users and/or escalation policies

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Resolve an incident or list of incidents

> The incident(s) must be currently open.  The user supplied must be a valid VictorOps user and a member of your organization.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Incidents`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Get an organization's on-call users

> Get all on-call uesrs/teams for your organization.<br/>
> <br/>
> This API may be called a maximum of 1 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### List routing keys with associated teams

> Retrieves a list of routing keys and associated teams.<br/>
> This API may be called a maximum of once a minute.

*Tags:* `Routing Keys`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### List the scheduled overrides

> List all the scheduled overrides on the organization<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Creates a new scheduled override

> Creates a new scheduled override. Start and end dates are in ISO8601 format. E.g. `2018-09-28'T'05:00:00Z`<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Deletes a scheduled override

> Deletes a scheduled override<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `publicId` - _required_ - The publicId of the scheduled override

### Get the specified scheduled override

> Get the specified scheduled override<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `publicId` - _required_ - The publicId of the scheduled override

### Get the specified scheduled override

> Get the specified scheduled override assignments

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `publicId` - _required_ - The publicId of the scheduled override

### Delete the scheduled override assignment

> Delete the scheduled override assignment

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `publicId` - _required_ - The publicId of the scheduled override
* `policySlug` - _required_ - The policySlug of the assignment

### Get the specified scheduled override assignment

> Get the specified scheduled override assignments

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `publicId` - _required_ - The publicId of the scheduled override
* `policySlug` - _required_ - The policySlug of the assignment

### Update the scheduled override assignment

> Update the scheduled override assignment

*Tags:* `Scheduled Overrides`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `publicId` - _required_ - The publicId of the scheduled override
* `policySlug` - _required_ - The policySlug of the assignment

### Get escalation policy info

> Retrieves a list of escalation policy information.<br/>
> This API may be called a maximum of once a minute

*Tags:* `Escalation Policies`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Get the available contact types

> Get the available contact types<br/>
> <br/>
> description: "Email Address", type: "email"<br/>
> description: "Phone Number", type: "phone"<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policy Values`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Get the available notification types

> Get the available notification types<br/>
> <br/>
> description: "Send a push notification to all my devices", type: "push"<br/>
> description: "Send an email to an email address", type: "email"<br/>
> description: "Send an SMS to a phone number", type: "sms"<br/>
> description: "Make a phone call to a phone number", type: "phone"<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policy Values`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Get the available timeout values

> Get the available timeout values<br/>
> <br/>
> description: "If still unacked after 1 minute", type: 1<br/>
> description: "If still unacked after 5 minutes", type: 5<br/>
> description: "If still unacked after 10 minutes", type: 10<br/>
> description: "If still unacked after 15 minutes", type: 15<br/>
> description: "If still unacked after 20 minutes", type: 20<br/>
> description: "If still unacked after 25 minutes", type: 25<br/>
> description: "If still unacked after 30 minutes", type: 30<br/>
> description: "If still unacked after 45 minutes", type: 45<br/>
> description: "If still unacked after 60 minutes", type: 60<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policy Values`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Create an on-call override (take on-call)

> Replaces a currently on-call user in the escalation policy with another.  In many cases, the policy slug<br/>
> will match the slug of the team that contains it.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `policy` - _required_ - The VictorOps policy 'slug'

### Get the user's paging policy

> Get all the paging policy steps for the user on the org associated with the API key<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Create a paging policy step

> Create a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Get a paging policy step

> Get a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `step` - _required_ - Paging policy step
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Create a rule for a paging policy step

> Create a rule for a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `step` - _required_ - Paging policy step
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Update a paging policy step

> Update a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `step` - _required_ - Paging policy step
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Delete a rule from a paging policy step

> Delete a rule from a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `step` - _required_ - Paging policy step
* `rule` - _required_ - Rule for a paging policy step
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Get a rule from a paging policy step

> Get a rule from a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `step` - _required_ - Paging policy step
* `rule` - _required_ - Rule for a paging policy step
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Update a rule for a paging policy step

> Update a rule for a paging policy step<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Personal Paging Policies`

#### Input Parameters
* `username` - _required_ - Your username
* `step` - _required_ - Paging policy step
* `rule` - _required_ - Rule for a paging policy step
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### List teams

> Get a list of teams for your organization.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Add a team

> Add a team to your organization.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Remove a team

> Remove a team from your organization.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to be deleted

### Retrieve information for a team

> Get the information for the specified team.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to fetch

### Update a team

> Update the designated team<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to be updated

### Retrieve a list of team admins for a team

> Get the team admins for the specified team.<br/>
> <br/>
> This API may be called a maximum of 30 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team

### Retrieve a list of members for a team

> Get the members for the specified team.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to fetch

### Add a team member

> Add a team member to your team.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to fetch

### Remove a team member

> Remove a team from your organization.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to be deleted
* `user` - _required_ - The team member username

### Get a team's on-call schedule

> __NOTE: This call is deprecated. Please use `GET /api-public/v2/team/{team}/oncall/schedule`.__<br/>
> <br/>
> Get the on-call schedule for a team, including on-call overrides.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team 'slug'
* `daysForward` - _optional_ - Days to include in returned schedule (30 max)
* `daysSkip` - _optional_ - Days to skip before computing schedule to return (90 max)
* `step` - _optional_ - Step of escalation policy (3 max)

### Create an on-call override (take on-call)

> __NOTE: This API call is deprecated. Please use `PATCH /api-public/v2/policies/{policy}/oncall/user`__<br/>
> <br/>
> Replaces a currently on-call user on the team with another.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team 'slug'

### Retrieve a list of escalation policies for a team

> Get the escalation policies for the specified team.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Escalation Policies` `Teams`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team to fetch

### List users

> Get a list of users for your organization<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Users`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Add a user

> Add a user to your organization<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Users`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key

### Remove a user

> Remove a user from your organization. If no replacement is specified, an empty JSON payload ("{}") is still required.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Users`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user to be deleted

### Retrieve information for a user

> Get the information for the specified user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Users`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user to fetch

### Update a user

> Update the designated user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `Users`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user to be updated

### Get a list of all contact methods for a user

> Get the contact methods for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Get a list of all contact devices for a user

> Get the contact methods for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Delete a contact device for a user

> Delete a contact device for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Get the indicated contact device for a user

> Get the indicated contact device for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Update a contact device for a user

> Update a contact device for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Get a list of all contact emails for a user

> Get the contact emails for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Create a contact emails for a user

> Create a contact email for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Delete a contact email for a user

> Delete the indicated contact email for the user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Get the indicated contact email for a user

> Get the indicated contact email for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Get a list of all contact phones for a user

> Get the contact phones for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Create a contact phones for a user

> Create a contact phone for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Delete a contact phone for a user

> Delete the indicated contact phone for the user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Get the indicated contact phone for a user

> Get the indicated contact phone for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Contact Methods`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `contactId` - _required_ - The unique contact identifier

### Get a user's on-call schedule

> __NOTE: This call is deprecated. Please use `GET /api-public/v2/user/{user}/oncall/schedule`.__<br/>
> <br/>
> Get the on-call schedule for a user for all teams, including on-call overrides.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `daysForward` - _optional_ - Days to include in returned schedule (30 max)
* `daysSkip` - _optional_ - Days to skip before computing schedule to return (90 max)
* `step` - _optional_ - Step of escalation policy (3 max)

### Get a list of paging policies for a user

> Get paging policies for a user<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `User Paging Policies`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID

### Retrieve the user's team membership

> This API may be called a maximum of 30 times per minute.

*Tags:* `Users`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user

### Get a team's on-call schedule

> Get the on-call schedule for a team, including on-call overrides.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team 'slug'
* `daysForward` - _optional_ - Days to include in returned schedule (30 max)
* `daysSkip` - _optional_ - Days to skip before computing schedule to return (90 max)
* `step` - _optional_ - Step of escalation policy (3 max)

### Get a user's on-call schedule

> Get the on-call schedule for a user for all teams the user is on, including on-call overrides.<br/>
> <br/>
> This API may be called a maximum of 15 times per minute.

*Tags:* `On-call`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `user` - _required_ - The VictorOps user ID
* `daysForward` - _optional_ - Days to include in returned schedule (30 max)
* `daysSkip` - _optional_ - Days to skip before computing schedule to return (90 max)
* `step` - _optional_ - Step of escalation policy (3 max)

### Get/search incident history

> __NOTE: This call is deprecated. Please use `GET /api-reporting/v2/incidents`.__<br/>
> <br/>
> Retrieve incident history for your company, searching over date ranges and with filtering options.  This is historical<br/>
> data, and may be up to 15 minutes behind real-time incident data.  By default, only resolved incidents will be returned.<br/>
> <br/>
> This API may be called a maximum of once a minute.<br/>
> <br/>
> Incident requests are paginated with a offset and limit query string parameters.<br/>
>   The query for incidents is run and offset records are skipped, after which limit records will be returned.<br/>
> <br/>
> The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.<br/>
> <br/>
> On return, the total number of records available for that query will be returned in the payload as 'total'.

*Tags:* `Reporting`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `offset` - _optional_ - The offset within the set of matching incidents
* `limit` - _optional_ - The maximum number of matching incidents to return (100 max)
* `entityId` - _optional_ - The entity ID involved  This is the unique identifier for the entity causing the incident.
* `incidentNumber` - _optional_ - The incident number as shown in VictorOps Multiple values and ranges are allowed: 4,5,20:50

* `startedAfter` - _optional_ - Return incidents started after this timestamp Specify the timestamp in ISO8601 format
* `startedBefore` - _optional_ - Find incidents started before this timestamp  Specify the timestamp in ISO8601 format
* `host` - _optional_ - The host involved in the incident Multiple values can be separated with commas.
* `service` - _optional_ - The service involved in the incident (if any) Multiple values can be separated with commas.
* `currentPhase` - _optional_ - The current phase of the incident "resolved", "triggered" or "acknowledged". Multiple values can be separated with commas.

### A list of shift changes for a team

> Returns a log of user shift changes for the specified team. This is historical<br/>
> data, and may be up to 15 minutes behind real-time log data.<br/>
> <br/>
> This API may be called a maximum of 6 times per minute.

*Tags:* `Reporting`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `team` - _required_ - The VictorOps team 'slug'
* `start` - _optional_ - Return shift changes occurring after this timestamp. The default is the start of the day at midnight. Specify the timestamp in ISO8601 format
* `end` - _optional_ - Return shift changes occurring before this timestamp. The default is the end of the day at 11:59:59. Specify the timestamp in ISO8601 format
* `userName` - _optional_ - The VictorOps user ID. Return shift changes occurring during the interval specified for this user. Without this parameter, all relevant users (with respect to the specified interval) are returned

### Get/search incident history

> Retrieve incident history for your company, searching over date ranges and with filtering options.<br/>
> <br/>
> This API may be called a maximum of once a minute.<br/>
> <br/>
> Incident requests are paginated with a offset and limit query string parameters.<br/>
>   The query for incidents is run and offset records are skipped, after which limit records will be returned.<br/>
> <br/>
> The default offset is 0 and the default limit is 20. The maximum value allowed for limit is 100.<br/>
> <br/>
> Unless specified otherwise with the parameter currentPhase, the response will only contain resolved incidents.<br/>
> <br/>
> On return, the total number of records available for that query will be returned in the payload as 'total'.

*Tags:* `Reporting`

#### Input Parameters
* `X-VO-Api-Id` - _required_ - Your API ID
* `X-VO-Api-Key` - _required_ - Your API Key
* `offset` - _optional_ - The offset within the set of matching incidents
* `limit` - _optional_ - The maximum number of matching incidents to return (100 max)
* `entityId` - _optional_ - The entity ID involved  This is the unique identifier for the entity causing the incident.
* `incidentNumber` - _optional_ - The incident number as shown in VictorOps Multiple values and ranges are allowed: 4,5,20:50

* `startedAfter` - _optional_ - Return incidents started after this timestamp Specify the timestamp in ISO8601 format
* `startedBefore` - _optional_ - Find incidents started before this timestamp  Specify the timestamp in ISO8601 format
* `host` - _optional_ - The host involved in the incident Multiple values can be separated with commas.
* `service` - _optional_ - The service involved in the incident (if any) Multiple values can be separated with commas.
* `currentPhase` - _optional_ - The current phase of the incident "resolved", "triggered" or "acknowledged". Multiple values can be separated with commas. By default, response contains only "resolved" incidents
* `routingKey` - _optional_ - The original routing of the incident

## License

**flow**ground :- Telekom iPaaS / victorops-com-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
