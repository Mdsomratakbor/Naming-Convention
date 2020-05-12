# C# Coding Standards and Naming Conventions
<table>
<thead>
<tr>
<th align="left">Object Name</th>
<th align="left">Notation</th>
<th align="right">Length</th>
<th align="left">Plural</th>
<th align="left">Prefix</th>
<th align="left">Suffix</th>
<th align="left">Abbreviation</th>
<th align="left">Char Mask</th>
<th align="left">Underscores</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Class name</td>
<td align="left">PascalCase</td>
<td align="right">128</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Constructor name</td>
<td align="left">PascalCase</td>
<td align="right">128</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Method name</td>
<td align="left">PascalCase</td>
<td align="right">128</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Method arguments</td>
<td align="left">camelCase</td>
<td align="right">128</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Local variables</td>
<td align="left">camelCase</td>
<td align="right">50</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Constants name</td>
<td align="left">PascalCase</td>
<td align="right">50</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Field name</td>
<td align="left">camelCase</td>
<td align="right">50</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">[A-z][0-9]</td>
<td align="left">Yes</td>
</tr>
<tr>
<td align="left">Properties name</td>
<td align="left">PascalCase</td>
<td align="right">50</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">[A-z][0-9]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Delegate name</td>
<td align="left">PascalCase</td>
<td align="right">128</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">Yes</td>
<td align="left">Yes</td>
<td align="left">[A-z]</td>
<td align="left">No</td>
</tr>
<tr>
<td align="left">Enum type name</td>
<td align="left">PascalCase</td>
<td align="right">128</td>
<td align="left">Yes</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">No</td>
<td align="left">[A-z]</td>
<td align="left">No</td>
</tr>
</tbody>
</table>

 **1. Do use PascalCasing for class names and method names:**</br>
 <pre><span class="pl-k">public</span> <span class="pl-k">class</span> <span class="pl-en">ClientActivity</span>
{
  <span class="pl-k">public</span> <span class="pl-k">void</span> <span class="pl-en">ClearStatistics</span>()
  {
    <span class="pl-c"><span class="pl-c">//</span>...</span>
  }
  <span class="pl-k">public</span> <span class="pl-k">void</span> <span class="pl-en">CalculateStatistics</span>()
  {
    <span class="pl-c"><span class="pl-c">//</span>...</span>
  }
}</pre>

**2. Do use camelCasing for method arguments and local variables:**
<pre><span class="pl-k">public</span> <span class="pl-k">class</span> <span class="pl-en">UserLog</span>
{
  <span class="pl-k">public</span> <span class="pl-k">void</span> <span class="pl-en">Add</span>(<span class="pl-en">LogEvent</span> <span class="pl-smi">logEvent</span>)
  {
    <span class="pl-k">int</span> <span class="pl-smi">itemCount</span> <span class="pl-k">=</span> <span class="pl-smi">logEvent</span>.<span class="pl-smi">Items</span>.<span class="pl-smi">Count</span>;
    <span class="pl-c"><span class="pl-c">//</span> ...</span>
  }
}</pre>
**3. Do not use Hungarian notation or any other type identification in identifiers**
<pre><span class="pl-c"><span class="pl-c">//</span> Correct</span>
<span class="pl-k">int</span> <span class="pl-smi">counter</span>;
<span class="pl-k">string</span> <span class="pl-smi">name</span>;    
<span class="pl-c"><span class="pl-c">//</span> Avoid</span>
<span class="pl-k">int</span> <span class="pl-smi">iCounter</span>;
<span class="pl-k">string</span> <span class="pl-smi">strName</span>;</pre>
**4. Do not use Screaming Caps for constants or readonly variables:**
<pre><span class="pl-c"><span class="pl-c">//</span> Correct</span>
<span class="pl-k">public</span> <span class="pl-k">const</span> <span class="pl-k">string</span> <span class="pl-smi">ShippingType</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>DropShip<span class="pl-pds">"</span></span>;
<span class="pl-c"><span class="pl-c">//</span> Avoid</span>
<span class="pl-k">public</span> <span class="pl-k">const</span> <span class="pl-k">string</span> <span class="pl-smi">SHIPPINGTYPE</span> <span class="pl-k">=</span> <span class="pl-s"><span class="pl-pds">"</span>DropShip<span class="pl-pds">"</span></span>;</pre>
**5. Use meaningful names for variables. The following example uses seattleCustomers for customers who are located in Seattle:**
<pre><span class="pl-k">var</span> <span class="pl-smi">seattleCustomers</span> <span class="pl-k">=</span> <span class="pl-k">from</span> <span class="pl-en">customer</span> <span class="pl-k">in</span> <span class="pl-smi">customers</span>
  <span class="pl-k">where</span> <span class="pl-smi">customer</span>.<span class="pl-smi">City</span> <span class="pl-k">==</span> <span class="pl-s"><span class="pl-pds">"</span>Seattle<span class="pl-pds">"</span></span> 
  <span class="pl-k">select</span> <span class="pl-smi">customer</span>.<span class="pl-smi">Name</span>;</pre>
  **6. Avoid using Abbreviations. Exceptions: abbreviations commonly used as names, such as Id, Xml, Ftp, Uri.**
  <pre><span class="pl-c"><span class="pl-c">//</span> Correct</span>
<span class="pl-en">UserGroup</span> <span class="pl-smi">userGroup</span>;
<span class="pl-en">Assignment</span> <span class="pl-smi">employeeAssignment</span>;     
<span class="pl-c"><span class="pl-c">//</span> Avoid</span>
<span class="pl-en">UserGroup</span> <span class="pl-smi">usrGrp</span>;
<span class="pl-en">Assignment</span> <span class="pl-smi">empAssignment</span>; 
<span class="pl-c"><span class="pl-c">//</span> Exceptions</span>
<span class="pl-en">CustomerId</span> <span class="pl-smi">customerId</span>;
<span class="pl-en">XmlDocument</span> <span class="pl-smi">xmlDocument</span>;
<span class="pl-en">FtpHelper</span> <span class="pl-smi">ftpHelper</span>;
<span class="pl-en">UriPart</span> <span class="pl-smi">uriPart</span>;</pre>
