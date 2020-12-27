## Example
<pre>
<apex:page docType="html-5.0" title="Output Link">
    <apex:outputText value="&lt;a href=&quot;http://www.example.com&quot;&gt;{0,date,MM/dd/yyyy}&lt;/a&gt;" escape="false">          
            <apex:param value="{!TODAY()}" />
            <a href="http://www.example.com">{!TEXT(MONTH(TODAY())) & '/' & TEXT(DAY(TODAY())) & '/' & TEXT(YEAR(TODAY()))}</a>
    </apex:outputText>
</apex:page>
</pre>

## References

* https://news.ycombinator.com/item?id=16461950
* https://lillesvin.net/posts/mixed-rendering-xss/
* https://github.com/dotboris/vuejs-serverside-template-xss
