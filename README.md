# rawDNS

RawDNS. It's PowerDNS. Doesn't offer more than that. Just is builded in a way to gave us more options on how to use and so we called it "rawDNS". 


This repo is created as a app which clients can use. We've Create the same idea for customer-panel but that's php-based not bash.

The usage of this is simple. 

* INSTALLATION.

* **1 .** **`git clone https://github.com/DopeHosting/rawDNS.git`**

* **2 .** **`cd rawDNS`**

* **3 .** **`mkdir /admin; mv ~/rawDNS/admin/mysql /admin/`**

* **4 .** **`nano /admin/mysql`**

~ Wrote your mysql credinals on it. (as for password use mysql password) And wrote your nameservers.

* **5 .** **`chmod +x install.sh; ./install.sh`**

---


* CLI.
* **1 .** **`mv ~/rawDNS/bin/rawdns /bin/; chmod +x /bin/rawdns`**

~ Host a Domain With your dns service.
* **2 .** **`rawdns create example.com`**

~ Get Domain ID.
* **3 .** **`rawdns id example.com`**

~ Create SOA (Without This You Domain Will not reach your server ip.) **1** = `example.com` **ID**
* **4 .** **`rawdns soa example.com 1`**

~ Create one record for this domain. (**1** = `example.com` **ID**)
* **5 .** **`rawdns rec 1 example.com 123.123.123.123 A 3600`**

~ Another One.
* **6 .** **`rawdns rec 1 www.example.com 123.123.123.123 A 3600`**

~ Delete domain and All records which this domain have.
* **7 .** **`rawdns del 1`**

~ Delete Single Record For One Domain.
* **8 .** **`raws rdel www.example.com`**

~ Another Delete ex.
* **9 .** **`raws rdel subdomain.example.com`**



---


# Footer.

* [HOME](http://dopehosting.com/)
* [Customer-Panel](https://dopeinfinity.io/)

How can i order? You can't as you can see our home page isn't live yet. Because we're working with our control panel. Because everything will be created by us. No CPanel/WHM. No Plesk Panel.

But To try our service on trial plan you can contact (raw@systemroot.me)
