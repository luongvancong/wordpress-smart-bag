## Lấy danh sách product stock status

```php
wc_get_product_stock_status_options()
```
**Danh sách stock status mặc định**

```php
array(
  'instock'     => __( 'In stock', 'woocommerce' ),
  'outofstock'  => __( 'Out of stock', 'woocommerce' ),
  'onbackorder' => __( 'On backorder', 'woocommerce' ),
)
```

## Kiểm tra sản phẩm có muốn quản lý stock không

```php
get_manage_stock() === true;
```

## Cập nhật số lượng stock quantity

```php
$product->set_manage_stock(true); 
$product->set_stock_quantity(0); 
$product->set_stock_status('outofstock');
$product->save();
```

