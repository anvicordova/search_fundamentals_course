# Week 1

1. Copy a subset of the data to `/workspace/datasets/sample`
    - cd /workspace/datasets
    - mkdir -p sample/product_data/products
    - cp product_data/products/products_0001_2570_to_430420.xml sample/product_data/products/

2. Index a subset of the data with  `./index-sample-data.sh`


## Opensearch

1. View existing indices 
    ```
    GET _cat/indices?v
    ```

2. Delete an index, ex: bbuy_products
    ```
    DELETE bbuy_products
    ```
3. See mappings of an index
    ```
    GET bbuy_products/_mapping
    ```

    or for a single field

    ```
    GET bbuy_products/_mapping/field/field_name
    ```
