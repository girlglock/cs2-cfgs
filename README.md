# cs2 cfg

## Launch Options

```
+exec_async autoexec -novconsole -disable_workshop_command_filtering -allow_third_party_software
```

<table>
<thead>
<tr><th>Flag</th><th>Description</th></tr>
</thead>
<tbody>
<tr>
<td nowrap><code>exec_async autoexec</code></td>
<td>Executes your autoexec on launch. <code>+exec_async</code> bypasses <code>-tools</code> alias restrictions. Can be replaced with regular <code>+exec</code> if not using <code>-tools</code></td>
</tr>
<tr>
<td nowrap><code>novconsole</code></td>
<td>Forces the Panorama console instead of the VConsole. Only relevant when running with <code>-tools</code> and total preference</td>
</tr>
<tr>
<td nowrap><code>disable_workshop_command_filtering</code></td>
<td>Allows aliased exec binds to function correctly on workshop maps.. ie <code>-vtest</code> ones</td>
</tr>
<tr>
<td nowrap><code>allow_third_party_software</code></td>
<td>Needed for obs and rivatuner etc</td>
</tr>
</tbody>
</table>
