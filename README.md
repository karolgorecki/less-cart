# Popup shoping cart module build on less
- - -
### should look like this
![cart look](https://raw.github.com/karolgorecki/less-cart/master/assets/cart-icon.png)

### how it looks:
![cart real look](https://raw.github.com/karolgorecki/less-cart/master/assets/cart-icon-css.png)

# Configuration options
* popup align to left/right side
* colors
* border radius
* arrow size/position

## Variables 
### Color
* @cart-button-bg - defines the background color of the cart button
* @main-box-border-color - defines the border color of the popup body
* @main-box-bg - defines the background color of the popup body
* @button-bg - defines the color of background checkout button
* @price-color - defines the color of the item prices

### Aligment
* @align - defines the aligment of the popup body (left/right)

### Sizes
* @inner-width - defines the width of the popup body
* @arrow-size - defines the arrow size
* @item-size - defines the image size and single item row

### Arrow position
* @inner-top-offset - defines the gap between cart button and the body
* @arrow-x-offset - defines the arrow position on the x axis

### Main box
* @main-box-border - definition for main box border
* @main-box-radius - definition for the border radius
* @main-box-shadow - definition for box shadow

# How to use

### html source
```html
<div class="cart-module">
	<span class="cart-button-text">My cart (1)</span>
	<div class="inner">
		<div class="main-box">
			<div class="item-box">

			<!-- Single product row -->
			<div class="item">
				<a href="#"><img src="http://lorempixum.com/32/32" alt=""></a>
				<div class="item-name"><a href="#">Some great product</a></div>
				<div class="price">$59,99</div>
				<a href="#" title="Remove product" class="remove-item">Remove</a>
			</div>

			<!-- Total amount -->
			<div class="total-box">
				<div class="subtotal">Subtotal: <b>$265,99</b></div>
				<div class="total">Total: <b>$2505,99</b></div>
				<div class="grandtotal">Grand total: <b>$2505,99</b></div>
			</div>

		</div>

		<!-- call2action buttons -->
		<div class="buttons">
			<a href="#" class="checkout-link">Go to Checkout</a>
			<a href="#" class="cart-link">Go to Cart</a>
		</div>
	</div>
</div>
```

### css source
```css
/* call the init on the cart module*/
.cart-module {
	#cart-button-popup > .init;
}
```