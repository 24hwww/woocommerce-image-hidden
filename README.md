# Woocommerce Image Hidden
## Plugin para Woocommerce que oculta las imagenes de la pagina tienda.
----

```
<?php
/*
Plugin Name: Woocommerce Image Hidden
Plugin URI: http://github.com/24hwww/woocommerce-image-hidden/
Description: Plugin para Woocommerce que oculta las imagenes de la pagina tienda.
Version: 1.0
Author: 24hwww
Author URI: http://github.com/24hwww/
License: Commercial
License URI: http://github.com/24hwww/woohidden-shop-image/
Text Domain: woocommerce-image-hidden

@author		 24hwww
@package	 Woocommerce Image Hidden
@since		 1.0

*/
if ( ! defined( 'ABSPATH' ) ) :
	exit; // Exit if accessed directly
endif;

/**
 * Check if WooCommerce is active
 * @since 1.0
 */
if ( in_array( 'woocommerce/woocommerce.php', apply_filters( 'active_plugins', get_option( 'active_plugins' ) ) ) ) :
remove_action( 'woocommerce_before_shop_loop_item_title', 'woocommerce_template_loop_product_thumbnail', 10 );
endif;
```
