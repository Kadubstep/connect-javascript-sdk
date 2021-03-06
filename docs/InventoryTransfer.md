# SquareConnect.InventoryTransfer

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **String** | A unique ID generated by Square for the [InventoryTransfer](#type-inventorytransfer). | [optional] 
**referenceId** | **String** | An optional ID provided by the application to tie the [InventoryTransfer](#type-inventorytransfer) to an external system. | [optional] 
**state** | **String** | The [InventoryState](#type-inventorystate) for the quantity of items being transfered. | [optional] 
**fromLocationId** | **String** | The Square ID of the [Location](#type-location) where the related quantity of items were tracked before the transfer. | [optional] 
**toLocationId** | **String** | The Square ID of the [Location](#type-location) where the related quantity of items were tracked after the transfer. | [optional] 
**catalogObjectId** | **String** | The Square generated ID of the [CatalogObject](#type-catalogobject) being tracked. | [optional] 
**catalogObjectType** | **String** | The [CatalogObjectType](#type-catalogobjecttype) of the [CatalogObject](#type-catalogobject) being tracked.Tracking is only supported for the &#x60;ITEM_VARIATION&#x60; type. | [optional] 
**quantity** | **String** | The number of items affected by the transfer as a decimal string. Fractional quantities are not supported. | [optional] 
**occurredAt** | **String** | A client-generated timestamp in RFC 3339 format that indicates when the transfer took place. For write actions, the &#x60;occurred_at&#x60; timestamp cannot be older than 24 hours or in the future relative to the time of the request. | [optional] 
**createdAt** | **String** | A read-only timestamp in RFC 3339 format that indicates when Square received the transfer request. | [optional] 
**source** | [**SourceApplication**](SourceApplication.md) | Read-only information about the application that initiated the inventory transfer. | [optional] 
**employeeId** | **String** | The Square ID of the [Employee](#type-employee) responsible for the inventory transfer. | [optional] 


<a name="StateEnum"></a>
## Enum: StateEnum


* `CUSTOM` (value: `"CUSTOM"`)

* `IN_STOCK` (value: `"IN_STOCK"`)

* `SOLD` (value: `"SOLD"`)

* `RETURNED_BY_CUSTOMER` (value: `"RETURNED_BY_CUSTOMER"`)

* `RESERVED_FOR_SALE` (value: `"RESERVED_FOR_SALE"`)

* `SOLD_ONLINE` (value: `"SOLD_ONLINE"`)

* `ORDERED_FROM_VENDOR` (value: `"ORDERED_FROM_VENDOR"`)

* `RECEIVED_FROM_VENDOR` (value: `"RECEIVED_FROM_VENDOR"`)

* `IN_TRANSIT_TO` (value: `"IN_TRANSIT_TO"`)

* `NONE` (value: `"NONE"`)

* `WASTE` (value: `"WASTE"`)

* `UNLINKED_RETURN` (value: `"UNLINKED_RETURN"`)




