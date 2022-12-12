# ionic-cap-volum-button-listner

Its will be used to listen volum button press in android ionic capastor

## Install

```bash
npm install ionic-cap-volum-button-listner
npx cap sync
```

## API

<docgen-index>

* [`addListener('volumeButtonPressed', ...)`](#addlistenervolumebuttonpressed)
* [`removeAllListeners()`](#removealllisteners)
* [Interfaces](#interfaces)
* [Type Aliases](#type-aliases)

</docgen-index>

<docgen-api>
<!--Update the source file JSDoc comments and rerun docgen to update the docs below-->

### addListener('volumeButtonPressed', ...)

```typescript
addListener(event: 'volumeButtonPressed', listenerFunc: VolumeButtonPressedListener) => Promise<PluginListenerHandle> & PluginListenerHandle
```

Listen for presses on the hardware volume buttons

| Param              | Type                                                                                |
| ------------------ | ----------------------------------------------------------------------------------- |
| **`event`**        | <code>'volumeButtonPressed'</code>                                                  |
| **`listenerFunc`** | <code><a href="#volumebuttonpressedlistener">VolumeButtonPressedListener</a></code> |

**Returns:** <code>Promise&lt;<a href="#pluginlistenerhandle">PluginListenerHandle</a>&gt; & <a href="#pluginlistenerhandle">PluginListenerHandle</a></code>

**Since:** 1.0.0

--------------------


### removeAllListeners()

```typescript
removeAllListeners() => Promise<void>
```

Removes all listeners for this plugin

**Since:** 1.0.0

--------------------


### Interfaces


#### PluginListenerHandle

| Prop         | Type                                      |
| ------------ | ----------------------------------------- |
| **`remove`** | <code>() =&gt; Promise&lt;void&gt;</code> |


### Type Aliases


#### VolumeButtonPressedListener

<code>({ direction, }: <a href="#volumebuttonpressed">VolumeButtonPressed</a>): void</code>


#### VolumeButtonPressed

<code>{ direction: 'up' | 'down' }</code>

</docgen-api>
