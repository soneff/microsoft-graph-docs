---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new OpenShift
{
	SchedulingGroupId = "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
	SharedOpenShift = new OpenShiftItem
	{
		Notes = "Inventory Management",
		OpenSlotCount = 5,
		DisplayName = "Field shift",
		StartDateTime = DateTimeOffset.Parse("2018-10-04T00:58:45.340Z"),
		EndDateTime = DateTimeOffset.Parse("2018-10-04T09:50:45.332Z"),
		Theme = ScheduleEntityTheme.White,
		Activities = new List<ShiftActivity>
		{
			new ShiftActivity
			{
				IsPaid = true,
				StartDateTime = DateTimeOffset.Parse("2018-10-04T00:58:45.340Z"),
				EndDateTime = DateTimeOffset.Parse("2018-10-04T01:58:45.340Z"),
				Code = "",
				DisplayName = "Lunch",
			},
		},
	},
	DraftOpenShift = null,
};
var result = await graphClient.Teams["{team-id}"].Schedule.OpenShifts["{openShift-id}"].PatchAsync(requestBody);


```