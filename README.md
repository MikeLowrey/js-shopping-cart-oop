# js-shopping-cart-oop
A javascript class to add, remove and increment products in the shopping cart. The class stores the shopping cart data in the local storage of the browser.

To add Product to Basket use c.addItem(product_id, quantity)
To remove Product from Basket use c.deleteItemFromCart(product_id)
To delelte the whole Cart c.deleteWholeCart()

To add increase, decrease, remove the quantity of an specific product you can implement custom function like:

    function addToBasket(data) {        
        c.addItem(data.dataset.id,1);          
    }

    function increaseProductInBasketById(data) {        
        let current_q = c.getItem(data.id);
        let new_q = (parseInt(current_q)+1);        
        c.addItem(data.id, new_q);
    }
    
    function removeItemFromBsketById(data) {        
        c.deleteItemFromCart(data.dataset.id);
    }
   
