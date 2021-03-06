# DocumentSnapshot

A DocumentSnapshot contains data read from a document in your Cloud Firestore database. The data can be extracted with `.data()` or `.get(<field>)` to get a specific field.

## Properties

### exists
[method]exists returns boolean;[/method]

Property of the DocumentSnapshot that signals whether or not the data exists. True if the document exists.

### id
[method]id returns string;[/method]

Property of the DocumentSnapshot that provides the document's ID.

### metadata
[method]metadata returns [ref firestore.SnapshotMetadata];[/method]

Metadata about the DocumentSnapshot, including information about its source and local modifications.

### ref
[method]ref returns [ref firestore.DocumentReference];[/method]

The DocumentReference for the document included in the DocumentSnapshot.

## Methods

### data
[method]data() returns Object;[/method]

Retrieves all fields in the document as an object.

### get
[method]get(fieldPath) returns any type or undefined;[/method]

| Parameter |         |
| --------- | ------- |
| fieldPath  | **string** or **[ref firestore.FieldPath]** <br /> The path (e.g. 'foo' or 'foo.bar') to a specific field. |


