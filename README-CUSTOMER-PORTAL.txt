SP PRINT PORTAL — CUSTOMER WORKSPACE UPDATE

CUSTOMER PANEL
- Open customer.html or choose Customer Login from the website header.
- Customer registration and login are available.
- WordPress-style customer workspace with a responsive sidebar:
  Dashboard, New Service Request, My Work / Requests, My Uploads,
  Download Center and My Profile.
- Dashboard shows total requests, awaiting review, in-progress work and
  ready/completed work.
- Service request form captures service, quantity, print type, size, delivery
  preference, urgency, instructions and multiple original files.
- Customers can see request status, work progress, shop notes and update history.
- Customers can download their submitted originals and completed files.
- Customers can edit their profile details.

OWNER / ADMIN PANEL
- Open admin.html or choose Admin Login from the website header.
- Existing owner dashboard and website management sections are retained.
- Print Requests / Work Queue lists the request details, customer contact,
  original uploaded files and a WhatsApp contact link.
- Manage Work lets the owner set Pending / Received, Processing, Ready for
  collection, Completed / Delivered or Cancelled, update progress from 0–100%,
  add a customer-facing note and upload a final delivery file.
- Uploaded final files are available to the customer in Download Center.

WHATSAPP
- Submitting a request opens WhatsApp with a pre-filled message containing
  request ID, customer contact, service details and uploaded file names.
- Website browsers do not allow a page to silently attach a local file to a
  WhatsApp message. The actual uploaded file is saved with the request in this
  browser's local storage and is downloadable from the admin request list.

IMPORTANT GITHUB PAGES / STATIC HOSTING LIMIT
- This is a plain HTML, CSS and JavaScript site. It does not require PHP.
- The customer accounts, requests, original files, final files and sessions are
  stored in the browser's localStorage. Customer and admin views can manage the
  same requests only when opened in the same browser profile/device.
- GitHub Pages alone cannot provide shared multi-device accounts, central file
  storage, secure private customer documents, or real-time notifications.
  For customers to register on their own phones and have every request appear
  in the owner's device, a shared backend (such as Supabase or Firebase) must
  be configured with project credentials and security rules. No backend keys
  were included in the supplied project, so this ZIP does not pretend that
  cross-device syncing is active.
- The admin password check is client-side JavaScript and is not strong
  server-side security. Do not use this static demo for sensitive identity
  document storage or public production accounts without a secure backend.
- Customer attachments and admin final files are limited to 1.2 MB each in this
  browser-only build to reduce localStorage quota failures.
