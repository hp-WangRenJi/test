# TVGuideAssessmentiOS
## External Libraries
In this demo, I use three external libraries.<br>
The first two are AFNetWorking and UIKit+AFNetworking. 
AFNetWorking is for the GET request to get data from server. 
UIKit+AFNetworking is to use the setImageWithURL function to set the ImageView in the table cell.
About several years ago, many applications choose to use ASIHTTPRequest but it has stopped updating for four years.
As ASIHTTPRequest is based on CFNetwork, AFNetWorking is based on NSURL, so ASI is little faster, 
however AFN encapsulates the data structure for JSON, XML, PList and Image data we don't need to implement SBJson.
So I think, if an application does not have many underlying customized demands, using AFNetworking is the best choice.<br>

The third one I use is SVProgressHD. 
I use this is simply because it is a clean and easy-to-use HUD meant to display the progress of an ongoing task on iOS, 
so once users' network are not very good, they won't feel boring waiting.
If designer wants something customized to suit the other design, I can create a new one and do not use this library.

## Suggestions
About suggestion on this page, I think for the main display view, only use table view is a little monotonous 
and the table view cell height is to small. 
Each cell seems to narrow. May be expand the cell with more infomation and a big image will increase the desire of clicking to see the details.
Also, use a page control to display some popular show images at the top of the table view is a better choice.
And a search bar at the top or a search button on the navigation bar is a better option than in the left view. 
As user have to first click the leftbutton on the navigation bar, and then click the search button.
Such as:<br>
![](https://photos-1.dropbox.com/t/2/AADMrKs5YbyGY3ssf8_ae70zDT1q_ZjLpeBNWGGj1NgPgA/12/128691490/jpeg/32x32/3/1459083600/0/2/example.jpg/ENKAi2MY6QEgASgB/lBoT5baMXr91OiGd8HgxWgKST7j0Xk_wY31Ulw7F6J8?size_mode=3&size=1024x768)
<br>
In the third page, I think may be adding more pictures on that button is better than just color and txt.
As '‘A picture is worth a thousand words'.<br>
Also I think, we may put some suggestions on the Search page.<br>
In the last page, I think the txt is too long, users don't like to read that.
So I think may be a small video is a better choice.

## Other thoughts
In this demo, I use the Model-View-ViewModel strcture to build the application. 
To put the business logic, data and validation in the ViewModel layer, and display in the Viewcontroller layer.
Whether the MVC, MVVM, MVCS or any other structure, there is no best one but only the most appropriate one for the project.
I think as long as we seperate the business logic, data, API request, database and display logic to make it clean, easy to maintain and iteration and suit for the project is the best structure.

