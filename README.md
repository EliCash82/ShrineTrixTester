# README.md

~~Ruby 2.3.3~~

~~Rails 5.0.7.2~~

Ruby 2.5.1

Rails 5.1.7

---

* Trix dynamic text editing [WORKING]
* Shrine basic image upload [WORKING]
* Drag Drop Image to Document Functionality [NOT WORKING]

---

ISSUES DISCOVERED:

This line of JS in `trix_uploads.js` is reliant on **Rails 5.1+** ( but less than 6.0), and I had been working with 
**Rails 5.0.x**:
`xhr.setRequestHeader("X-CSRF-Token", Rails.csrfToken());`
