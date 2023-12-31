# CS50W - Project 1 - Auctions Website

This repository contains the second assignment of CS50 Web Programming, which involves creating a simple clone of an auction website, similar to eBay. The project is built using Python's web framework Django, along with HTML and CSS.

## YouTube Video
For a detailed explanation of the project's required specifications, you can watch a video overview here: [Project 1 Video](https://youtu.be/bjnKtMNB-7Q)

## Assignment Specification
- **Models**: The application must include at least three models in addition to the `User` model: one for auction listings, one for bids, and one for comments on auction listings. The structure of these models, including the fields and field types, is left to your discretion. You can introduce additional models if necessary.
- **Create Listing**: Users should be able to access a page to create a new listing. This involves specifying a title, a text-based description, and the starting bid. Optionally, users can also provide an image URL for the listing and assign a category (e.g., Fashion, Toys, Electronics, Home, etc.).
- **Active Listings Page**: The default route of the web application should display all currently active auction listings. For each active listing, the minimum information shown should include the title, description, current price, and an image (if provided).
- **Listing Page**: Clicking on a listing should direct users to a dedicated page for that listing. Here, users can view comprehensive details about the listing, including its current price.
  - If a user is signed in, they should have the option to add the item to their "Watchlist." If the item is already on the watchlist, the user should be able to remove it.
  - Authenticated users should be able to place bids on the item. Bids must meet certain criteria, such as being higher than the starting bid and any existing bids. In case of invalid bids, an appropriate error message should be displayed.
  - The user who created the listing and is signed in should be able to "close" the auction from this page. Closing the auction designates the highest bidder as the winner and renders the listing inactive.
  - On a closed listing page, if the signed-in user has won the auction, the page should indicate so.
  - Authenticated users should be able to leave comments on the listing page, and all comments should be visible.
- **Watchlist**: Signed-in users can access a Watchlist page that displays all listings they have added to their watchlist. Clicking on a listing should take the user to that item's specific page.
- **Categories**: A page displaying all listing categories should be available. Clicking on a category name should lead to a page showing all active listings within that category.
- **Django Admin Interface**: The Django admin interface should allow site administrators to perform operations such as viewing, adding, editing, and deleting listings, comments, and bids.
