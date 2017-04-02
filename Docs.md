<a name="dynamojo"></a>

## dynamojo : <code>object</code>
Dynamojo

A simplified nodejs client for DynamoDB on AWS.

**Kind**: global namespace  
**Version**: v1  

* [dynamojo](#dynamojo) : <code>object</code>
    * [.config(options)](#dynamojo.config)
    * [.get(table, id, [fields], callback)](#dynamojo.get)
    * [.getByKey(table, indexName, key, value, [fields], callback)](#dynamojo.getByKey)
    * [.list(table, callback)](#dynamojo.list)
    * [.listByKey(table, indexName, key, value, [qf], callback)](#dynamojo.listByKey)
    * [.update(table, id, update, callback)](#dynamojo.update)

<a name="dynamojo.config"></a>

### dynamojo.config(options)
Configure AWS credentials and endpoint

**Kind**: static method of <code>[dynamojo](#dynamojo)</code>  

| Param | Type | Description |
| --- | --- | --- |
| options | <code>object</code> | Your custom aws configure options |

<a name="dynamojo.get"></a>

### dynamojo.get(table, id, [fields], callback)
Get an item by primary id.

**Kind**: static method of <code>[dynamojo](#dynamojo)</code>  

| Param | Type | Description |
| --- | --- | --- |
| table | <code>string</code> | The DynamoDB TableName |
| id | <code>string</code> | The primary index value. Usually a the id UUID. |
| [fields] | <code>object</code> | (optional) Only return these fields. |
| callback | <code>callback</code> | The callback that handles the response. |

<a name="dynamojo.getByKey"></a>

### dynamojo.getByKey(table, indexName, key, value, [fields], callback)
Get an item by primary id.

**Kind**: static method of <code>[dynamojo](#dynamojo)</code>  

| Param | Type | Description |
| --- | --- | --- |
| table | <code>string</code> | The DynamoDB TableName |
| indexName | <code>string</code> | The DynamoDB IndexName |
| key | <code>string</code> | DynamoDB key name |
| value | <code>string</code> | DynamoDB key value |
| [fields] | <code>object</code> | (optional) Only return these fields. |
| callback | <code>callback</code> | The callback that handles the response. |

<a name="dynamojo.list"></a>

### dynamojo.list(table, callback)
Lists all items in a table

**Kind**: static method of <code>[dynamojo](#dynamojo)</code>  

| Param | Type | Description |
| --- | --- | --- |
| table | <code>string</code> | DynamoDB TableName |
| callback | <code>callback</code> | The callback that handles the response. |

<a name="dynamojo.listByKey"></a>

### dynamojo.listByKey(table, indexName, key, value, [qf], callback)
Lists all items in a table

**Kind**: static method of <code>[dynamojo](#dynamojo)</code>  

| Param | Type | Description |
| --- | --- | --- |
| table | <code>string</code> | The DynamoDB TableName |
| indexName | <code>string</code> | The DynamoDB IndexName |
| key | <code>string</code> | DynamoDB key name |
| value | <code>string</code> | DynamoDB key value |
| [qf] | <code>object</code> | (optional) An optional query, passed as an object. |
| callback | <code>callback</code> | The callback that handles the response. |

<a name="dynamojo.update"></a>

### dynamojo.update(table, id, update, callback)
Update values for a single item by primary index.

**Kind**: static method of <code>[dynamojo](#dynamojo)</code>  

| Param | Type | Description |
| --- | --- | --- |
| table | <code>string</code> | The DynamoDB TableName |
| id | <code>string</code> | The primary index value. Usually a the id UUID. |
| update | <code>object</code> | The new item values, passed as an object. |
| callback | <code>callback</code> | The callback that handles the response. |
