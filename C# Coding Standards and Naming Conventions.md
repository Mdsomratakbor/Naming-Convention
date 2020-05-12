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

<h4><a id="user-content-1-do-use-pascalcasing-for-class-names-and-method-names" class="anchor" aria-hidden="true" href="#1-do-use-pascalcasing-for-class-names-and-method-names"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>1. Do use PascalCasing for class names and method names:</h4>
