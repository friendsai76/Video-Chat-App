# Video-Chat-App---Django
A Video Chat Web Application Using Django and JavaScprit.

Create and activate a python virtual environment and then django for this project.
Open your terminal or command prompt and navigate to your Django project directory. We will use mysite as the project name for this tutorial.
Enter “pip install websockets” in terminal install websockets.

Create urls.py under chat app and specify the path in urlpatterns and then include it to main app urls.

Create consumers.py file so our clients going to connect our server using websocket.
The way we implement a chat room using django-channels is by leveraging a feature called groups.
 Where the messages can be sent through all channels in the group to their respective peers.
Most of the code here is for send our SDP to other peers.

![image](https://user-images.githubusercontent.com/85016767/127934206-a29b39e7-0a03-46bc-aa2d-2a0a6558488f.png)



Specify In-Memory channel layer / Redis Channel Layer in Settings.py.

Later on, write the code Accordingly in JS file using WebRTC , data channels and Websocket or refer to the Code files that been sent and the final Output is:

![image](https://user-images.githubusercontent.com/85016767/127934164-e00e4e6e-70a9-490e-b9d8-927045dd76f7.png)

  Limitations:
  As more peers join it get slow.
  It is only upto development level. For production level we can using redis-channel layers.
  It works only when 2 devices on same network.
  Stun and turn servers are recommended to connect on different networks
  '*' is for allowing all hosts & it is not recommended for production level.
