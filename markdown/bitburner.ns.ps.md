<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [NS](./bitburner.ns.md) &gt; [ps](./bitburner.ns.ps.md)

## NS.ps() method

List running scripts on a server.

**Signature:**

```typescript
ps(host?: string): ProcessInfo[];
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  host | string | _(Optional)_ Host address of the target server. If not specified, it will be the current server’s IP by default. |

**Returns:**

[ProcessInfo](./bitburner.processinfo.md)<!-- -->\[\]

Array with general information about all scripts running on the specified target server.

## Remarks

RAM cost: 0.2 GB

Returns an array with general information about all scripts running on the specified target server.

## Example 1


```ts
// NS1:
var scripts = ps("home");
for (var i = 0; i < scripts.length; ++i) {
    tprint(scripts[i].filename + ' ' + scripts[i].threads);
    tprint(scripts[i].args);
}
```

## Example 2


```ts
// NS2:
const ps = ns.ps("home");
for (let script of ps) {
    ns.tprint(`${script.filename} ${script.threads}`);
    ns.tprint(script.args);
}
```

