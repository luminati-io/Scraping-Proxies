# Bright Data's Scraping Proxies

[![Promo](https://github.com/luminati-io/LinkedIn-Scraper/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.com/proxy-types/residential-proxies) 

## About Bright Data
Bright Data is an award winning leading proxy provider that serves over 20,000 customers world wide. Over 100M proxy IPs, best-in-class technology and the ability to target any country, city, carrier & ASN make our proxy services a top choice for developers.

## Residential Proxies
Experience seamless scraping with Bright Data's [industry-leading residential proxies](https://brightdata.com/proxy-types/residential-proxies), designed to provide precise targeting, unmatched stability, and rapid response times.

- **72M+ Residential IPs**
- **Sticky and rotating sessions**
- **99.95% success rate**
- **HTTP(S) & SOCKS5 support**
- **Geo-location targeting (Free)**

## Key Features
- **Global Coverage**: Residential proxies available in [195 countries](https://brightdata.com/locations).
- **High Success Rates**: Achieve up to 99.95% success in your scraping projects.
- **Fast Response**: Average response time of ~0.7 seconds.
- **Ethically Sourced**: All proxies are sourced with explicit user consent.
- **Unlimited Concurrent Sessions**: Scale your operations without limitations.

## Pricing Plans
- **Pay As You Go**: $8.4/GB, no monthly commitment required.
- **Monthly Subscriptions**:
  - **69 GB**: $7.14/GB, $499/month.
  - **158 GB**: $6.3/GB, $999/month.
  - **339 GB**: $5.88/GB, $1999/month.
  - **Enterprise Plans**: Custom solutions available for large-scale needs.

Sign up and receive a dollar-for-dollar match on your first deposit, up to $500!

## Getting Started with Residential Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Use our APIs or Control Panel to manage IPs and configurations.
3. **Supported Languages**: Quick start examples provided for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'residential', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
             'https': 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 33335);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-residential", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:33335");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-residential", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-residential:"[your password]"@brd.superproxy.io:33335',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:33335 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## Mobile Proxies
Access the internet as a real mobile user with Bright Data's [mobile proxy network](https://brightdata.com/proxy-types/mobile-proxies), featuring millions of 3G, 4G, and 5G IPs from around the world.

- **7,000,000+ Mobile IPs**
- **3G/4G/5G mobile IPs**
- **99.99% Uptime with 24/7 support**
- **Geo-location targeting (Free)**

## Key Features
- **Global Reach**: Access mobile IPs across [195 countries](https://brightdata.com/locations).
- **High Success Rates**: Achieve up to 99.9% success in data collection and testing tasks.
- **Real Mobile Connections**: Mobile IPs sourced from real devices on genuine networks.
- **Unlimited Scaling**: Scale with concurrent sessions and high-availability infrastructure.
- **Carrier-Level Targeting**: Target by specific carriers for in-depth, accurate insights.

## Pricing Plans
- **Pay As You Go**: $8.4/GB with no monthly commitment.
- **Monthly Subscriptions**:
  - **69 GB**: $7.14/GB, $499/month + VAT.
  - **158 GB**: $6.3/GB, $999/month + VAT.
  - **339 GB**: $5.88/GB, $1999/month + VAT.
  - **Enterprise Plans**: Custom pricing and packages available.

Sign up today and get a dollar-for-dollar match on your first deposit, up to $500!

## Getting Started with Mobile Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Use APIs or the Bright Data Control Panel to manage IPs and configurations.
3. **Supported Languages**: Quick start examples provided for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'mobile', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-mobile", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-mobile", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-mobile:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell 

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-mobile:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## ISP Proxies
Utilize Bright Data's extensive [ISP proxy network](https://brightdata.com/proxy-types/isp-proxies) for secure, stable, and high-speed data collection with IPs sourced directly from ISPs.

- **700,000+ ISP IPs**
- **Static Residential IPs** with long-term stability
- **99.9% success rate**
- **HTTP(S) & SOCKS5 support**
- **Free Country-Level Targeting**

## Key Features
- **Global Reach**: Access ISP IPs across [multiple countries](https://brightdata.com/locations).
- **High Success Rates**: Up to 99.9% success in accessing websites.
- **Fast and Stable**: Low latency and reliable uptime with 99.99% network availability.
- **Exclusive IP Access**: Dedicated IPs for consistent connections.
- **Ethically Sourced**: All ISP proxies are obtained directly from ISPs and are compliant with GDPR and CCPA.

## Pricing Plans
- **Pay As You Go**: $15/GB for monthly commitment-free usage.
- **Monthly Subscriptions - Shared**:
  - **10 IPs**: $1.80/IP, $18/month + VAT.
  - **100 IPs**: $1.45/IP, $145/month + VAT.
  - **500 IPs**: $1.40/IP, $700/month + VAT.
  - **1,000 IPs**: $1.30/IP, $1300/month + VAT.
  - **Enterprise Plans**: Custom solutions for extensive data collection needs.
 
- **Monthly Subscriptions - Dedicated**:
  - **10 IPs**: $3.50/IP, $35/month + VAT.
  - **100 IPs**: $2.75/IP, $275/month + VAT.
  - **500 IPs**: $2.60/IP, $1300/month + VAT.
  - **1,000 IPs**: $2.50/IP, $2500/month + VAT.
  - **Enterprise Plans**: Custom solutions for extensive data collection needs.
 
- **Monthly Subscriptions - Pay/GB**:
  - $12.75/GB, $499/month + VAT.
  - $11.25/GB, $999/month + VAT.
  - $10.50/GB, $1999/month + VAT.
  - **Enterprise Plans**: Custom solutions for extensive data collection needs.


## Getting Started with ISP Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Manage IPs and configurations via Bright Data's Control Panel or API.
3. **Supported Languages**: Quick start guides provided for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'isp', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-isp", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-isp", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-isp:"[your password]"@brd.superproxy.io:22225',
})
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-isp:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## Datacenter Proxies
Leverage Bright Data's extensive [datacenter proxy network](https://brightdata.com/proxy-types/datacenter-proxies) with unmatched scale and speed for reliable data collection and web scraping.

- **770,000+ Datacenter IPs**
- **[Shared](https://brightdata.com/solutions/shared-proxies) and [Dedicated](https://brightdata.com/solutions/dedicated-proxies) IP Options**
- **~0.24s Average Response Time**
- **HTTP(S) & [SOCKS5](https://brightdata.com/solutions/socks5-proxies) Support**
- **Free Country-Level Targeting**

## Key Features
- **Global Reach**: Access datacenter IPs across [98 countries](https://brightdata.com/locations).
- **High Success Rates**: Achieve up to 99.9% success in scraping tasks.
- **Fast and Reliable**: 99.99% network uptime and rapid connection speeds.
- **Customizable Options**: Choose between shared or dedicated IPs based on your needs.
- **Unlimited Scaling**: Support for concurrent sessions without restrictions.

## Pricing Plans
- **Pay As You Go**: $0.6/GB for a monthly commitment-free experience.
- **Monthly Subscriptions - Shared**:
  - **10 IPs**: $1.40/IP, $14/month + VAT.
  - **100 IPs**: $1.00/IP, $100/month + VAT.
  - **500 IPs**: $0.95/IP, $475/month + VAT.
  - **1,000 IPs**: $0.90/IP, $900/month + VAT.
  - **Enterprise Plans**: Tailored solutions for large-scale data collection.

- **Monthly Subscriptions - Dedicated**:
  - **10 IPs**: $2.20/IP, $22/month + VAT.
  - **100 IPs**: $1.70/IP, $170/month + VAT.
  - **500 IPs**: $1.50/IP, $750/month + VAT.
  - **1,000 IPs**: $1.30/IP, $1300/month + VAT.
  - **Enterprise Plans**: Tailored solutions for large-scale data collection.


- **Monthly Subscriptions - Pay/GB**:
  - $0.51/GB, $499/month + VAT.
  - $0.45/GB, $999/month + VAT.
  - $0.42/GB, $1999/month + VAT.
  - **Enterprise Plans**: Tailored solutions for large-scale data collection.

Sign up and get a dollar-for-dollar match on your first deposit, up to $500!

## Getting Started with Datacenter Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Manage IPs and configurations with APIs or the Bright Data Control Panel.
3. **Supported Languages**: Quick start guides available for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'datacenter', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-datacenter", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-datacenter", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
    })
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```
### Join [Bright Data](https://brightdata.com) now and see why we are the industry leader. 
