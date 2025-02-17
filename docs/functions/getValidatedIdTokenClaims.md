# Function: getValidatedIdTokenClaims()

[💗 Help the project](https://github.com/sponsors/panva)

Support from the community to continue maintaining and improving this module is welcome. If you find the module useful, please consider supporting the project by [becoming a sponsor](https://github.com/sponsors/panva).

***

▸ **getValidatedIdTokenClaims**(`ref`): [`IDToken`](../interfaces/IDToken.md) \| `undefined`

Returns ID Token claims validated during [processRefreshTokenResponse](processRefreshTokenResponse.md) or
[processDeviceCodeResponse](processDeviceCodeResponse.md). To optionally validate its JWS Signature use
[validateApplicationLevelSignature](validateApplicationLevelSignature.md)

## Parameters

| Parameter | Type | Description |
| ------ | ------ | ------ |
| `ref` | [`TokenEndpointResponse`](../interfaces/TokenEndpointResponse.md) | Value previously resolved from [processRefreshTokenResponse](processRefreshTokenResponse.md), [processBackchannelAuthenticationGrantResponse](processBackchannelAuthenticationGrantResponse.md) or [processDeviceCodeResponse](processDeviceCodeResponse.md). |

## Returns

[`IDToken`](../interfaces/IDToken.md) \| `undefined`

JWT Claims Set from an ID Token, or undefined if there is no ID Token in `ref`.
