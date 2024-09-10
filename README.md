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

### How it works...

I am replacing an entire HTML form with one specialized textarea. It accepts data structured in TOML. 
E.g. If you want to send the following JSON to the server; where value of each field has to be obtained from the user: e.g.
```
{name: "xyz", age: 63, address: {first: "adsfadfdfd", city: "Mumbai", country: "India"},...}
```
It can even have nested objects ... then you can express it in TOML as:

```
name = "xyz"
age = 63
address.first = "adsfadfdfd"
address.city = "Mumbai"
address.country = "India"
....
```

In above case the page can get filled with input boxes, etc. In case of my TOML editor I can capture all that in one textarea with prompts on the left side. And you give just the values (i.e. after the equal-to sign of each line) into the textarea.It can even handle validation and provide additional help for each line the caret happens to be on.

The textarea has ruled lines to guide the user, and won't accept newlines and wont allow you to delete newlines (thus preventing badly formatted TOML) It behaves like a set of inputs one below the other. Works quite well on small screens. My server even handles the TOML without strings quoted. My server adds the required quotes where absent. So it is quite natural and easy to type into that textarea.

You can simply load the given HTML file into a browser and you can see it in action. I believe in rapid agile development, so this is just the first of possibly many more iterations.

I will create other kinds of front-ends too; as and when I get the time.

Enjoy.
Best wishes.
