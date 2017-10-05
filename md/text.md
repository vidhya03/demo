## Below contents are render using markdown syntax 

![](https://gist.githubusercontent.com/vidhya03/efbfcb973f8997c16e73f6fb8b246942/raw/23a868e9e37f59a72403516d76e993fae7152aae/02-petstore-api-with-txt.jpg)

The Dingo API package is meant to provide you, the developer, with a set of tools to help you easily and quickly build your own API. While the goal of this package is to remain as flexible as possible it still won't cover all situations and solve all problems.
##Access via
 OAuth![OAuth](https://gist.githubusercontent.com/vidhya03/efbfcb973f8997c16e73f6fb8b246942/raw/92721ab04221ad39905986208cec3049a0a18132/01-oauth-small-76x76.png)
 APIKey![APIKey](https://gist.githubusercontent.com/vidhya03/efbfcb973f8997c16e73f6fb8b246942/raw/a50b77c7ce972a48c334dc43fc9f2a3476dbcd43/01-key-74x76.png)

## Features

This package provides tools for the following, and more:

- Content Negotiation
- Multiple Authentication Adapters
- API Versioning
- Rate Limiting
- Response Transformers and Formatters
- Error and Exception Handling
- Internal Requests
- API Blueprint Documentation

## Documentation

Please refer to our extensive [Wiki documentation](https://github.com/dingo/api/wiki) for more information.

## Support

For answers you may not find in the Wiki, avoid posting issues. Feel free to ask for support on the dedicated [Slack](https://larachat.slack.com/messages/api/) room. Make sure to mention **@jasonlewis** so he is notified.

## License

This package is licensed under the [BSD 3-Clause license](http://opensource.org/licenses/BSD-3-Clause).
## Sample code for Java client
```java
import java.io.IOException;
import javax.ws.rs.core.MediaType;
import javax.ws.rs.core.UriBuilder;
import org.apache.http.client.ClientProtocolException;
import com.sun.jersey.api.client.Client;
import com.sun.jersey.api.client.ClientResponse;
import com.sun.jersey.api.client.WebResource;
import com.sun.jersey.api.client.config.ClientConfig;
import com.sun.jersey.api.client.config.DefaultClientConfig;
import com.sun.jersey.api.representation.Form;
public class Test {
 public static void main(String[] args) throws ClientProtocolException, IOException {
  ClientConfig config = new DefaultClientConfig();
  Client client = Client.create(config);
  WebResource service = client.resource(UriBuilder.fromUri('http://restUrl').build());
  Form form = new Form();
  form.add('name1', 'value1');
  form.add('name2', 'value1');
  ClientResponse response = service.path('restPath').path('resourcePath').
  type(MediaType.APPLICATION_FORM_URLENCODED).post(ClientResponse.class, form);
  System.out.println('Response ' + response.getEntity(String.class));
 }
}
```





<h2 id="htmltag"> Below contents are render using html </h2>




<p><img src="https://gist.githubusercontent.com/vidhya03/efbfcb973f8997c16e73f6fb8b246942/raw/23a868e9e37f59a72403516d76e993fae7152aae/02-petstore-api-with-txt.jpg" alt="" /></p>

<p>The Dingo API package is meant to provide you, the developer, with a set of tools to help you easily and quickly build your own API. While the goal of this package is to remain as flexible as possible it still won't cover all situations and solve all problems.</p>

<h2 id="accessvia">Access via</h2>

<p>OAuth<img src="https://gist.githubusercontent.com/vidhya03/efbfcb973f8997c16e73f6fb8b246942/raw/92721ab04221ad39905986208cec3049a0a18132/01-oauth-small-76x76.png" alt="OAuth" />
 APIKey<img src="https://gist.githubusercontent.com/vidhya03/efbfcb973f8997c16e73f6fb8b246942/raw/a50b77c7ce972a48c334dc43fc9f2a3476dbcd43/01-key-74x76.png" alt="APIKey" /></p>

<h2 id="features">Features</h2>

<p>This package provides tools for the following, and more:</p>

<ul>
<li>Content Negotiation</li>

<li>Multiple Authentication Adapters</li>

<li>API Versioning</li>

<li>Rate Limiting</li>

<li>Response Transformers and Formatters</li>

<li>Error and Exception Handling</li>

<li>Internal Requests</li>

<li>API Blueprint Documentation</li>
</ul>

<h2 id="documentation">Documentation</h2>

<p>Please refer to our extensive <a href="https://github.com/dingo/api/wiki">Wiki documentation</a> for more information.</p>

<h2 id="support">Support</h2>

<p>For answers you may not find in the Wiki, avoid posting issues. Feel free to ask for support on the dedicated <a href="https://larachat.slack.com/messages/api/">Slack</a> room. Make sure to mention <strong>@jasonlewis</strong> so he is notified.</p>

<h2 id="license">License</h2>

<p>This package is licensed under the <a href="http://opensource.org/licenses/BSD-3-Clause">BSD 3-Clause license</a>.</p>

<h2 id="samplecodeforjavaclient">Sample code for Java client</h2>

<pre><code class="java language-java">import java.io.IOException;
import javax.ws.rs.core.MediaType;
import javax.ws.rs.core.UriBuilder;
import org.apache.http.client.ClientProtocolException;
import com.sun.jersey.api.client.Client;
import com.sun.jersey.api.client.ClientResponse;
import com.sun.jersey.api.client.WebResource;
import com.sun.jersey.api.client.config.ClientConfig;
import com.sun.jersey.api.client.config.DefaultClientConfig;
import com.sun.jersey.api.representation.Form;
public class Test {
 public static void main(String[] args) throws ClientProtocolException, IOException {
  ClientConfig config = new DefaultClientConfig();
  Client client = Client.create(config);
  WebResource service = client.resource(UriBuilder.fromUri('http://restUrl').build());
  Form form = new Form();
  form.add('name1', 'value1');
  form.add('name2', 'value1');
  ClientResponse response = service.path('restPath').path('resourcePath').
  type(MediaType.APPLICATION_FORM_URLENCODED).post(ClientResponse.class, form);
  System.out.println('Response ' + response.getEntity(String.class));
 }
}
</code></pre>