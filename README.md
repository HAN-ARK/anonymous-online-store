# Anonymous Online Store Application built with MERN Stack  
[Working Demo](https://anonymous-store.herokuapp.com/)
  
# Manulife Team 116 members  
Hanbyul Park  
Donika Morina  
Jananaen Selvapaskaran  
Kiet Do  
Muhammad Umair Ahsan  
Pui Hei Yan  

## Features  
* Guest check out
* Create new user  
* Log In & Out
* Add and remove one quantity of an item  
* Remove all quantities of an item  
* Edit the quantity of the items in real time  
* Calculate the total including the shipping automatically (if chosen)  


# Built with  
This project was made possible due to  
* React  
* MongoDB  
* Express  
* NodeJS  
* Multer  
* GridFS  
  
  
# Back-end Documentation  
<details>
<summary> Click to open up the documentation </summary>  

```
Tested Routes



TESTED means the route is tested and safe to use
TESTED? means the route is still in testing and can't ensure it will work
VendorId is the same as user's id. In early development, vendor model was separate and later merging with user side caused this to exist.



req: section means required section to be included with http request
req:key represents explanation for value: identifier for key



Unless specified, all the required sections are string.
Exceptions are specified here:
NAME : TYPE
price number




User Side (inside of users.js)



USER ACCOUNT



GET:    'users/          '   TESTED  'get all the users  ' req:
GET:    'users/get/:id   '   TESTED  'get one user       ' req: user id
POST:   'users/add       '   TESTED  'add a new user     ' req:key -> user email:email, username:username, password:password
POST:   'users/login     '   TESTED  'login existing user' req:key -> user email:email, user password:password
DELETE: 'users/delete/:id'   TESTED  'delete a user      ' req:key -> user id




USER & CART



POST:  'users/addItem    '   TESTED  'add an item       ' req:key -> user's id:userId, product id:productId
POST:  'users/removeItem '   TESTED  'delete item       ' req:key -> user's id:userId, product id:productId
POST:  'users/removeAll  '   TESTED  'delete all items  ' req:key -> user's id:userId, product id:productId



USER REVIEW PAGE
POST:  'users/total      '   TESTED  'total cost in cart' req: user id:userId
                                                return:key -> total cost:total, tax value:plusTax
POST:  'users/checkout   '   TESTED  'reset cart & cost ' req: user id:userId




Item Side (inside of items.js)



GET:    'items/          ' TESTED 'get all the items ' req:
GET:    'items/get/:id   ' TESTED 'get one item      ' req: item id
POST:   'items/add       ' TESTED 'add a item        ' req:key -> image file:img, vendorId:id, itemname:name,
                                                       description:desc, price in number:price
GET:    'items/image/:id ' TESTED 'get one image     ' req: image id
DELETE: 'items:id        ' TESTED 'delete one item   ' req: target item id  
```
</details>  

# Project Version Management 
Not all of backend implementations are linked in front end. Finishing full implementation is going to be the future plan.  

## Production  
[Production Version](https://github.com/HAN-ARK/anonymous-online-store)  
  
## Development
[Dev Version](https://github.com/KietDo0602/anonymous-store)  

