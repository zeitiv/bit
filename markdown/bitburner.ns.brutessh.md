<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [bitburner](./bitburner.md) &gt; [NS](./bitburner.ns.md) &gt; [brutessh](./bitburner.ns.brutessh.md)

## NS.brutessh() method

Runs BruteSSH.exe on a server.

**Signature:**

```typescript
brutessh(host: string): void;
```

## Parameters

|  Parameter | Type | Description |
|  --- | --- | --- |
|  host | string | Hostname of the target server. |

**Returns:**

void

## Remarks

RAM cost: 0.05 GB

Runs the BruteSSH.exe program on the target server. BruteSSH.exe must exist on your home computer.

## Example 1


```ts
// NS1:
brutessh("foodnstuff");
```

## Example 2


```ts
// NS2:
ns.brutessh("foodnstuff");
```

