# ShopTodo — Shopping Cart

> Specification for the workshop exercise.
> Target application: **https://arrangility.github.io/shoptodo-workshop/**
> Scope for today: **the shopping cart only.** Product listing, checkout, order history, todo and profile are out of scope.

## 1. Purpose

A signed-in user collects products in a cart before checking out.

**The cart is the user's working set.** Adding, changing the quantity and removing must all be reflected immediately, and what the user sees must match what is actually held.

## 2. Roles

The application ships with demo accounts. **The cart belongs to the signed-in user.**

| Role | Cart |
|---|---|
| Standard user | Has their own cart |
| Admin | Has their own cart |

⚠ One user must never see another user's cart.

## 3. Language

The interface can be switched between **English and Japanese** at any time.

## 4. Acceptance criteria

### 4.1 Add to cart

| # | Given | When | Then |
|---|---|---|---|
| A-1 | The user is signed in and the cart is empty | They add a product to the cart | The cart shows 1 item |
| A-2 | The cart contains at least one item | They open the cart | The cart total is greater than zero |

### 4.2 Change quantity

| # | Given | When | Then |
|---|---|---|---|
| Q-1 | The cart contains a product | The user increases the quantity | The quantity shown for that product increases |

### 4.3 Remove from cart

| # | Given | When | Then |
|---|---|---|---|
| R-1 | The cart contains a product | The user removes that product | A confirmation is shown |

### 4.4 Cart and language

| # | Given | When | Then |
|---|---|---|---|
| L-1 | The cart contains a product | The user switches the language | The interface language changes |

## 5. Out of scope for this exercise

Checkout, payment, order history, todo, profile, product search and category filtering.
