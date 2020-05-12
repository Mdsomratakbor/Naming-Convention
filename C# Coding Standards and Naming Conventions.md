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
