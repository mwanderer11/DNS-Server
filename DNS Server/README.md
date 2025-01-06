# Project 6

To complete this project, our approach was to first start by being able to parse the zone file for the SOA record and to retreive a list of all the local records. Next, we implemented the logic to parse A records, CNAME records, MX records, and NS records appropriately. This included resolving glue records for NS responses, finding corresponding A records when handling a CNAME record, etc. After responding locally was complete, we then implemented forwarding the query to the root ip address and then recursive forwarding. Finally, after that was done, we implemented the features that provided more enhancements such as bailiwick checking, running multiple client requests parallel through threading, and caching. 

The main challenges we faced were in becoming familiar enough with the content of the DNS responses, types of responses, and flags. Additionally, recursive forwarding was challenging, because it took some trial and error to figure out how to parse the NS records and A records for forwarding. 



We tested our code by running the provided config files individually to ensure that our code worked as expected.
