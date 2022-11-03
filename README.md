# First Interfaction Frontend Framework (FIFF) - AngularJS1

## Getting Started
https://github.com/edwinbernadus/first-interaction-frontend-framework


## Snippet List
- hint_create_button
````javascript
// hint_create_button
<!-- // hint_create_button -->
<button ng-click="changePage()">Change Page</button>
````
- hint_open_new_page
````javascript
// hint_open_new_page
window.location.href = "/list_page.html";
````
- hint_loading_webservice
````javascript
let url = "https://jsonplaceholder.typicode.com/albums"

// hint_loading_webservice
let output = await axios.get(url);
$app.result = output.data;
````
- hint_show_loading_indicator
````javascript
// hint_show_loading_indicator
$app.isLoading = true;
````
- hint_show_webservice_result_on_list
````javascript
<!-- // hint_show_webservice_result_on_list-->
<li ng-repeat="item in result">
    <div>{{item.title}}</div>
    <button ng-click="inquiryInfo(item)">Info</button>
</li>
````
- hint_button_on_list
````javascript
<!-- //hint_button_on_list-->
<button ng-click="inquiryInfo(item)">Info</button>
````
- hint_show_detail_item_on_alert
````javascript
// hint_show_detail_item_on_alert
let msg = item.id.toString() + "-" + item.title;
alert(msg)
````