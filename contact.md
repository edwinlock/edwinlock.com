---
layout: default
title: Contact
image: map.svg
caption: "A map of the British Isles with Oxford highlighted."
---

## Get in touch

If you have any questions, or if you would like to have a chat, please contact me using the form below.

<form action="{{ site.formurl }}" method="POST" class="mt-4 text-left">
<div class="form-row">
<input type="hidden" name="_subject" value="Contact request via personal website">
<div class="col-md form-group">
<label for="Name">Name</label>
<input type="text" class="form-control" id="Name" placeholder="Name">
</div>
<div class="col-md form-group">
<label for="Email">Email</label>
<input type="email" name="_replyto" class="form-control" id="Email" placeholder="Email address"
required>
</div>
</div>
<div class="form-group">
<textarea class="form-control" name="Message" rows="4" placeholder="Message…" required></textarea>
</div>
<button class="btn btn-outline-secondary" type="submit" value="Send">Send</button>
</form>
