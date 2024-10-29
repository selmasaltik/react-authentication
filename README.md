# Authentication
***User Signup & Login***

- **How Authentication Works** In React Apps
- **Implementing** User Authentication
- Adding Authentication **Persistence & Auto-Logout**

**Authentication is needed if content should be *protected***

i.e., if content should not be accessible by everyone

**[Getting Permission](https://www.canva.com/design/DAGU_tUY7wI/gfLPgEbIY5zdUBx3561v2g/view?utm_content=DAGU_tUY7wI&utm_campaign=designshare&utm_medium=link&utm_source=editor)**

**How Does Authentication Work?**

***Client and server can’t just exchange a “Yes”***

Any client could simply send a request to our backend that “tells” the backend that we previously were granted access

***Server-side Sessions***

- Store unique identifier on server, send same identifier to client
- Client sends identifier along with requests to protected resources
- Server can then check if the identifier is valid (= previously issued by server to client)

***Authentication Tokens***

- Create (but not store) “permission” token on server & send it to the client
- Client attaches token to future requests for protected resources
- Server can then verify the attached token

***[Working with Decoupled Backends](https://www.canva.com/design/DAGU_x8yXKk/H_KUBRNvR9SrIjEWpU2WhA/view?utm_content=DAGU_x8yXKk&utm_campaign=designshare&utm_medium=link&utm_source=editor)***
