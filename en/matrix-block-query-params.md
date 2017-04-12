Matrix Block Query Params
=========================

Param              | Accepts                                   | Description
------------------ | ----------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------
`addOrderBy`       | `string\|array\|Expression`               | Adds additional ORDER BY columns to the query
`addSelect`        | `string\|array\|Expression`               | Add more columns to the SELECT part of the query
`ancestorDist`     | `int\|null`                               | The maximum number of levels that results may be separated from `ancestorOf`
`ancestorOf`       | `int\|ElementInterface\|null`             | The element (or its ID) that results must be an ancestor of
`andWhere`         | `string\|array`                           | Adds an additional WHERE condition to the existing one
`archived`         | `bool`                                    | Whether to return only archived elements
`asArray`          | `bool`                                    | Whether to return each element as an array
`contentTable`     | `string\|null`                            | The content table that will be joined by this query
`customFields`     | `FieldInterface[]\|null`                  | The fields that may be involved in this query
`dateCreated`      | `mixed`                                   | When the resulting elements must have been created
`dateUpdated`      | `mixed`                                   | When the resulting elements must have been last updated
`descendantDist`   | `int\|null`                               | The maximum number of levels that results may be separated from `descendantOf`
`descendantOf`     | `int\|ElementInterface\|null`             | The element (or its ID) that results must be a descendant of
`elementType`      | `string\|null`                            | The name of the `ElementInterface` class
`enabledForSite`   | `bool`                                    | Whether the elements must be enabled for the chosen site
`fieldId`          | `int\|int[]\|string\|false\|null`         | The field ID(s) that the resulting Matrix blocks must belong to
`fixedOrder`       | `bool`                                    | Whether results should be returned in the order specified by `id`
`id`               | `int\|int[]\|false\|null`                 | The element ID(s)
`indexBy`          | `string\|callable`                        | The name of the column by which the query results should be indexed by
`level`            | `mixed`                                   | The element’s level within the structure
`limit`            | `int`                                     | Maximum number of records to be returned
`nextSiblingOf`    | `int\|ElementInterface\|null`             | The element (or its ID) that the result must be the next sibling of
`offset`           | `int`                                     | Zero-based offset from where the records are to be returned
`orWhere`          | `string\|array`                           | Adds an additional WHERE condition to the existing one
`orderBy`          | `array`                                   | How to sort the query results
`owner`            | `ElementInterface`                        | Sets the `ownerId` and `ownerSiteId` params based on a given element
`ownerId`          | `int\|int[]\|null`                        | The owner element ID(s) that the resulting Matrix blocks must belong to
`ownerLocale`      | `string\|string[]`                        | Sets the `ownerLocale` param
`ownerSite`        | `string\|string[]\|Site`                  | Sets the `ownerSiteId` param based on a given site(s)’s handle(s)
`ownerSiteId`      | `int\|string\|null`                       | The site ID that the resulting Matrix blocks must have been defined in, or ':empty:' to find blocks without an owner site ID
`positionedAfter`  | `int\|ElementInterface\|null`             | The element (or its ID) that the results must be positioned after
`positionedBefore` | `int\|ElementInterface\|null`             | The element (or its ID) that the results must be positioned before
`prevSiblingOf`    | `int\|ElementInterface\|null`             | The element (or its ID) that the result must be the previous sibling of
`ref`              | `string\|string[]\|null`                  | The reference code(s) used to identify the element(s)
`relatedTo`        | `int\|array\|ElementInterface\|null`      | The element relation criteria
`search`           | `string\|array\|SearchQuery\|null`        | The search term to filter the resulting elements by
`select`           | `array`                                   | The columns being selected
`siblingOf`        | `int\|ElementInterface\|null`             | The element (or its ID) that the results must be a sibling of
`site`             | `string\|Site`                            | Sets the `siteId` param based on a given site(s)’s handle
`siteId`           | `int\|null`                               | The site ID that the elements should be returned in
`slug`             | `string\|string[]\|null`                  | The slug that resulting elements must have
`status`           | `string\|string[]\|null`                  | The status(es) that the resulting elements must have
`structureId`      | `int\|false\|null`                        | The structure ID that should be used to join in the structureelements table
`title`            | `string\|string[]\|null`                  | The title that resulting elements must have
`type`             | `string\|string[]\|MatrixBlockType\|null` | Sets the `typeId` param based on a given block type(s)’s handle(s)
`typeId`           | `int\|int[]\|null`                        | The block type ID(s) that the resulting Matrix blocks must have
`uid`              | `string\|string[]\|null`                  | The element UID(s)
`uri`              | `string\|string[]\|null`                  | The URI that the resulting element must have
`where`            | `string\|array`                           | Query condition
`with`             | `string\|array\|null`                     | The eager-loading declaration
`with`             | `string\|array\|null`                     | The eager-loading declaration