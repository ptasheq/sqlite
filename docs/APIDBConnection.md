<p align="center"><br><img src="https://user-images.githubusercontent.com/236501/85893648-1c92e880-b7a8-11ea-926d-95355b8175c7.png" width="128" height="128" /></p>
<h2 align="center">API DB CONNECTION DOCUMENTATION</h2>
<p align="center"><strong><code>@capacitor-community/sqlite</code></strong></p>
<p align="center">
  SQLite DB Connection Wrapper</p>

## Methods Index

<docgen-index>

* [`getConnectionDBName()`](#getconnectiondbname)
* [`open()`](#open)
* [`close()`](#close)
* [`getUrl()`](#geturl)
* [`getVersion()`](#getversion)
* [`execute(...)`](#execute)
* [`query(...)`](#query)
* [`run(...)`](#run)
* [`executeSet(...)`](#executeset)
* [`isExists()`](#isexists)
* [`isDBOpen()`](#isdbopen)
* [`isTable(...)`](#istable)
* [`delete()`](#delete)
* [`createSyncTable()`](#createsynctable)
* [`setSyncDate(...)`](#setsyncdate)
* [`getSyncDate()`](#getsyncdate)
* [`exportToJson(...)`](#exporttojson)
* [Interfaces](#interfaces)

</docgen-index>

## API DB Connection Wrapper

<docgen-api class="custom-css">
<!--Update the source file JSDoc comments and rerun docgen to update the docs below-->

SQLiteDBConnection Interface

### getConnectionDBName()

```typescript
getConnectionDBName() => string
```

Get SQLite DB Connection DB name

**Returns:** <code>string</code>

**Since:** 2.9.0 refactor

--------------------


### open()

```typescript
open() => Promise<void>
```

Open a SQLite DB Connection

**Since:** 2.9.0 refactor

--------------------


### close()

```typescript
close() => Promise<void>
```

Close a SQLite DB Connection

**Since:** 2.9.0 refactor

--------------------


### getUrl()

```typescript
getUrl() => Promise<capSQLiteUrl>
```

Get Database Url

**Returns:** <code>Promise&lt;<a href="#capsqliteurl">capSQLiteUrl</a>&gt;</code>

**Since:** 3.3.3-4

--------------------


### getVersion()

```typescript
getVersion() => Promise<capVersionResult>
```

Get the a SQLite DB Version

**Returns:** <code>Promise&lt;<a href="#capversionresult">capVersionResult</a>&gt;</code>

**Since:** 3.2.0

--------------------


### execute(...)

```typescript
execute(statements: string, transaction?: boolean | undefined) => Promise<capSQLiteChanges>
```

Execute SQLite DB Connection Statements

| Param             | Type                 |
| ----------------- | -------------------- |
| **`statements`**  | <code>string</code>  |
| **`transaction`** | <code>boolean</code> |

**Returns:** <code>Promise&lt;<a href="#capsqlitechanges">capSQLiteChanges</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### query(...)

```typescript
query(statement: string, values?: any[] | undefined) => Promise<capSQLiteValues>
```

Execute SQLite DB Connection Query

| Param           | Type                | Description |
| --------------- | ------------------- | ----------- |
| **`statement`** | <code>string</code> |             |
| **`values`**    | <code>any[]</code>  | (optional)  |

**Returns:** <code>Promise&lt;<a href="#capsqlitevalues">capSQLiteValues</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### run(...)

```typescript
run(statement: string, values?: any[] | undefined, transaction?: boolean | undefined) => Promise<capSQLiteChanges>
```

Execute SQLite DB Connection Raw Statement

| Param             | Type                 | Description |
| ----------------- | -------------------- | ----------- |
| **`statement`**   | <code>string</code>  |             |
| **`values`**      | <code>any[]</code>   | (optional)  |
| **`transaction`** | <code>boolean</code> |             |

**Returns:** <code>Promise&lt;<a href="#capsqlitechanges">capSQLiteChanges</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### executeSet(...)

```typescript
executeSet(set: capSQLiteSet[], transaction?: boolean | undefined) => Promise<capSQLiteChanges>
```

Execute SQLite DB Connection Set

| Param             | Type                        |
| ----------------- | --------------------------- |
| **`set`**         | <code>capSQLiteSet[]</code> |
| **`transaction`** | <code>boolean</code>        |

**Returns:** <code>Promise&lt;<a href="#capsqlitechanges">capSQLiteChanges</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### isExists()

```typescript
isExists() => Promise<capSQLiteResult>
```

Check if a SQLite DB Connection exists

**Returns:** <code>Promise&lt;<a href="#capsqliteresult">capSQLiteResult</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### isDBOpen()

```typescript
isDBOpen() => Promise<capSQLiteResult>
```

Check if a SQLite database is opened

**Returns:** <code>Promise&lt;<a href="#capsqliteresult">capSQLiteResult</a>&gt;</code>

**Since:** 3.0.0-beta.5

--------------------


### isTable(...)

```typescript
isTable(table: string) => Promise<capSQLiteResult>
```

Check if a table exists

| Param       | Type                |
| ----------- | ------------------- |
| **`table`** | <code>string</code> |

**Returns:** <code>Promise&lt;<a href="#capsqliteresult">capSQLiteResult</a>&gt;</code>

**Since:** 3.0.0-beta.5

--------------------


### delete()

```typescript
delete() => Promise<void>
```

Delete a SQLite DB Connection

**Since:** 2.9.0 refactor

--------------------


### createSyncTable()

```typescript
createSyncTable() => Promise<capSQLiteChanges>
```

Create a synchronization table

**Returns:** <code>Promise&lt;<a href="#capsqlitechanges">capSQLiteChanges</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### setSyncDate(...)

```typescript
setSyncDate(syncdate: string) => Promise<void>
```

Set the synchronization date

| Param          | Type                |
| -------------- | ------------------- |
| **`syncdate`** | <code>string</code> |

**Since:** 2.9.0 refactor

--------------------


### getSyncDate()

```typescript
getSyncDate() => Promise<string>
```

Get the synchronization date

**Returns:** <code>Promise&lt;string&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### exportToJson(...)

```typescript
exportToJson(mode: string) => Promise<capSQLiteJson>
```

Export the given database to a JSON Object

| Param      | Type                |
| ---------- | ------------------- |
| **`mode`** | <code>string</code> |

**Returns:** <code>Promise&lt;<a href="#capsqlitejson">capSQLiteJson</a>&gt;</code>

**Since:** 2.9.0 refactor

--------------------


### Interfaces


#### capSQLiteUrl

| Prop      | Type                | Description    |
| --------- | ------------------- | -------------- |
| **`url`** | <code>string</code> | a returned url |


#### capVersionResult

| Prop          | Type                | Description     |
| ------------- | ------------------- | --------------- |
| **`version`** | <code>number</code> | Number returned |


#### capSQLiteChanges

| Prop          | Type                                        | Description                               |
| ------------- | ------------------------------------------- | ----------------------------------------- |
| **`changes`** | <code><a href="#changes">Changes</a></code> | a returned <a href="#changes">Changes</a> |


#### Changes

| Prop          | Type                | Description                                          |
| ------------- | ------------------- | ---------------------------------------------------- |
| **`changes`** | <code>number</code> | the number of changes from an execute or run command |
| **`lastId`**  | <code>number</code> | the lastId created from a run command                |


#### capSQLiteValues

| Prop         | Type               | Description                      |
| ------------ | ------------------ | -------------------------------- |
| **`values`** | <code>any[]</code> | the data values list as an Array |


#### capSQLiteSet

| Prop            | Type                | Description                      |
| --------------- | ------------------- | -------------------------------- |
| **`statement`** | <code>string</code> | A statement                      |
| **`values`**    | <code>any[]</code>  | the data values list as an Array |


#### capSQLiteResult

| Prop         | Type                 | Description                                   |
| ------------ | -------------------- | --------------------------------------------- |
| **`result`** | <code>boolean</code> | result set to true when successful else false |


#### capSQLiteJson

| Prop         | Type                                              | Description           |
| ------------ | ------------------------------------------------- | --------------------- |
| **`export`** | <code><a href="#jsonsqlite">JsonSQLite</a></code> | an export JSON object |


#### JsonSQLite

| Prop            | Type                     | Description                                           |
| --------------- | ------------------------ | ----------------------------------------------------- |
| **`database`**  | <code>string</code>      | The database name                                     |
| **`version`**   | <code>number</code>      | The database version                                  |
| **`encrypted`** | <code>boolean</code>     | Set to true (database encryption) / false             |
| **`mode`**      | <code>string</code>      | * Set the mode ["full", "partial"]                    |
| **`tables`**    | <code>JsonTable[]</code> | * Array of Table (<a href="#jsontable">JsonTable</a>) |
| **`views`**     | <code>JsonView[]</code>  | * Array of View (<a href="#jsonview">JsonView</a>)    |


#### JsonTable

| Prop           | Type                       | Description                                                 |
| -------------- | -------------------------- | ----------------------------------------------------------- |
| **`name`**     | <code>string</code>        | The database name                                           |
| **`schema`**   | <code>JsonColumn[]</code>  | * Array of Schema (<a href="#jsoncolumn">JsonColumn</a>)    |
| **`indexes`**  | <code>JsonIndex[]</code>   | * Array of Index (<a href="#jsonindex">JsonIndex</a>)       |
| **`triggers`** | <code>JsonTrigger[]</code> | * Array of Trigger (<a href="#jsontrigger">JsonTrigger</a>) |
| **`values`**   | <code>any[][]</code>       | * Array of Table data                                       |


#### JsonColumn

| Prop             | Type                | Description                         |
| ---------------- | ------------------- | ----------------------------------- |
| **`column`**     | <code>string</code> | The column name                     |
| **`value`**      | <code>string</code> | The column data (type, unique, ...) |
| **`foreignkey`** | <code>string</code> | The column foreign key constraints  |
| **`constraint`** | <code>string</code> | the column constraint               |


#### JsonIndex

| Prop        | Type                | Description                                                                                                             |
| ----------- | ------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **`name`**  | <code>string</code> | The index name                                                                                                          |
| **`value`** | <code>string</code> | The value of the index can have the following formats: email email ASC email, MobileNumber email ASC, MobileNumber DESC |
| **`mode`**  | <code>string</code> | the mode (Optional) UNIQUE                                                                                              |


#### JsonTrigger

| Prop            | Type                | Description                  |
| --------------- | ------------------- | ---------------------------- |
| **`name`**      | <code>string</code> | The trigger name             |
| **`timeevent`** | <code>string</code> | The trigger time event fired |
| **`condition`** | <code>string</code> | The trigger condition        |
| **`logic`**     | <code>string</code> | The logic of the trigger     |


#### JsonView

| Prop        | Type                | Description               |
| ----------- | ------------------- | ------------------------- |
| **`name`**  | <code>string</code> | The view name             |
| **`value`** | <code>string</code> | The view create statement |

</docgen-api>
