# Setup a DMARC Record

These instructions apply to cPanel only. If you need to do it on BPWeb, please update these instructions afterwards :)

1. Login to WHM (cPanel)
2. Search for "Edit DNS Zone"
3. Select the domain you're working on
4. Scroll down to "Add New Entries Below this Line"
5. Input the following:

In the first box, enter `_DMARC`, leave the second and then select `TXT` as the record type. In the box that appears to the right, paste `"v=DMARC1; p=quarantine; rua=mailto:<email>; ruf=mailto:<email>"`

**Important!** _Make sure you change `<email>` to the appropriate email address for reports or this will not function as expected._
