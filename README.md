# HTMX-FrontEnd
Here are some frontend examples for productive, rapid use of HTMX.

To begin with I developed a simple TOML "Editor" by working on a simple HTML Textarea 

### But why?

I was tired of creating front end input boxes, checkboxes, etc. and the complications
and time involved in them. Then I thought how about emulating a simple ruled paper?
After all, when we fill data manually (i.e. without a computer) we simply tear
a ruled paper and enter the data systematically one below the other on those lines.

So as a start, here is a simple method by which the user can send a TOML data 
to a server -- and TOML is quite good to capture a lot of complex JSON obj.

According to me, this is simple and quite useful. Your experience may vary.
This was written in a day, and so expect some errors. But I think I have
tested this reasonably well. 

The actual docs are in the HTML source: The source has the force, Luke.
Read ALL the comments and I think you should be good to go.

This HTMX-TOML editor is quite useful for Pocketbase servers. I can 
create and update Pocketbase collections records quite well with this.
It is agnostic to the database structure one may use at the server.
In fact, it is agnostic to Pocketbase too frankly -- it should work 
especially well with any backend that accepts intricate 
JSON for creating/updating database records.  

I mentioned Pocketbase because that is one technology I really like 
and this was tested in that backend: I can easily get back to the 
rest of the things I do, instead of being stuck in coding.

I will create other kinds of front-ends too; as and when I get the time.

Enjoy.
Best wishes.
