---
layout: post
---
Example of custom function. 

You can use any library or any HTTP method to ferch data from remote server

```
<script type="text/javascript">
    function ajaxDataProviderFunction(){
        return $.ajax({
            dataType: 'json',
            url: 'https://raw.githubusercontent.com/kupolua/web-presentation/master/json/db.json',
            success: function(jsonData){
                return jsonData;
            }
        });
    }
</script>
```
```
data-provider-function="ajaxDataProviderFunction"
```

*Please pay attention that we're returning asynchronous method which returns data when making async call
