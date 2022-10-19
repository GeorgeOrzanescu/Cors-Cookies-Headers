# How to play with this

 - clone the repo
 - start the server ( npm run dev)
 - go to localhost:5555 ( use this for CORS requests )
 - open another tab on 127.0.01:5555 ( this is same origin location )

IMPORTANT :  they are basically the same but the browser sees them like different origins allowing 
us to test CORS policies

# How it works

 - in index.html we have the following functions:
   - fSetLocal (DOES not perform a fetch request) set's cookie directly in browser
   - fDelLocal (DOES not perform a fetch request) deletes the cookie from the browser
   <-------------------------------------------------------------------------------------------------------->
   - fAdd makes a fetch request to the server to add a new cookie in the response back to the browser
   - fDel makes a fetch request to the server to delete a cookie (server sets the cookie age to 0 to remove the cookie)

U can play with them to test different CORS and cookie settings