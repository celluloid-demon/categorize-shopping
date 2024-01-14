Context
---

In the provided JSON object, the key "TAG_NAME" describes what type of goods the grocery list items are, the key "EXAMPLE_INPUT" describes a list of two random shopping items of that type (plus a random md5 hash as a unique identifier for each item), and the key "EXAMPLE_OUTPUT" describes how those list items look as an array of json objects.

Example JSON data
---

```
{

	"TAG_NAME":"Alcohol",

	"EXAMPLE_INPUT":[

		"Whiskey (id: 3e792e7e273e87ac325f0221b8a6cc6a)",
		"Vodka (id: 96e7a37d619aa29c0de41a13016ac6d9)"
		
	],

	"EXAMPLE_OUTPUT":[

		{"id": "3e792e7e273e87ac325f0221b8a6cc6a", "tag":"<GROCERIES-PREFIX><SEPARATOR><TAG-NAME>", "item":"Whiskey"},
		{"id": "96e7a37d619aa29c0de41a13016ac6d9", "tag":"<GROCERIES-PREFIX><SEPARATOR><TAG-NAME>", "item":"Vodka"}

	]

}
```

Request
---

Using that json data as an example, create a NEW json object if the object's "TAG_NAME" key were set to "<TAG-NAME>".

Additional Rules
---

- Indent using tabs.
- List only two items.
- Give each item a random md5 hash as a unique identifier (and store in each item's "id" field).
