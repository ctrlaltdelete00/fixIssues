Documentation Error - Fixed

https://github.com/jupyter/notebook/issues/603
--------------------------------------------------------------------------------------------------------------------------------
Original file:

https://github.com/jupyter/notebook/blob/b8b66332e2023e83d2ee04f83d8814f567e01a4e/notebook/static/notebook/js/quickhelp.js

Quickhelp.js : Fix is labeled on line 142
   function humanize_key(key){
142        //andreas entry for documentation fix
143         if (key.length === 1){
144             return key.toLowerCase();
145         }
146        key = humanize_map[key.toLowerCase()]||key;
147        if (key.indexOf(',') === -1){
148            return  ( special_case[key] ? special_case[key] :
149		    key.charAt(0).toUpperCase() + key.slice(1) );
        }
    }

*****TO BUILD (and fix this error) *****
Replace your quickhelp js with the file I have uploaded
If you want to find where my change is in the file → ctrl-f “andrea”
