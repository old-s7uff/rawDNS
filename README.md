# rawDNS

RawDNS. It's PowerDNS. Doesn't offer more than that. Just is builded in a way to gave us more options on how to use and so we called it "rawDNS". 


This repo is created as a app when clients can use. We use the same idea but php based not bash. 

The usage of this is simple. 

* Installation.
**1 .** **`git clone https://github.com/DopeHosting/rawDNS.git`**
**2 .** **`cd rawDNS`**
**3 .** **`mkdir /admin; mv ~/rawDNS/admin/mysql /admin/`**
**4 .** **`nano /admin/mysql`**
~ Wrote your mysql credinals on it. (as for password use whatever you want that will be used for mysql)
**5 .** **`chmod +x install.sh; ./install.sh`**

* CLI.
**1 .** **`mv ~/rawDNS/bin/rawdns; chmod +x /bin/rawdns`**

~ Host a Domain With your dns service.
* **1 .** **`rawdns create example.com`**

~ Get Domain ID.
* **2 .** **`rawdns id example.com`**

~ Create SOA (Without This You Domain Will not reach your server ip.) 1 = example.com ID
* **3 .** **`rawdns soa example.com 1`**

~ Create one record for this domains. (1 = example.com ID)
* **4 .** **`rawdns rec 1 example.com 123.123.123.123 A 3600`**

~ Another One.
* **5 .** **`rawdns rec 1 www.example.com 123.123.123.123 A 3600`**

~ Delete domain and All records which this domain have.
* **6 .** **`rawdns del 1`**

~ Delete Single Record For One Domain.
* **7 .** **`raws rdel www.example.com`**

~ Another Delete ex.
* **8 .** **`raws rdel subdomain.example.com`**



---


# Footer.

* [HOME](http://dopehosting.com/)
* [Customer-Panel](https://dopeinfinity.io/)

How can i order? You can't as you can see our home page isn't live yet. Because we're working with our control panel. Because everything will be created by us. No CPanel/WHM. No Plesk Panel.

But To try our service on trial plan you can contact (raw@systemroot.me)
