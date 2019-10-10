CREATE TABLE segmentation_templates (
    invoice_id                bigint,
    product_id                bigint,
    amount                    bigint,
    customer                  varchar,
    created_on                timestamp,
    
    PRIMARY KEY (invoice_id, product_id, created_on)
) WITH CLUSTERING ORDER BY (created_on DESC);