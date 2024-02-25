My public key: tpknam1qrd6884v4s9fcfxzdgj8qef6rmeam9re974njjlwflhdpvffwfjnvwceh6e

My moniker: Sined222

My channels:  
Namada channel-415 <-> channel-5886 Osmosis

My namada ibc wallet: sined222ibc tnam1qptx8tgf5dja847g88lyw2nym72p3fp38qy2224f  
My osmosis wallet: osmo_wallet osmo1e95jeru3nz4z4yz9s7va4wtc57rmgc3rrt7sep

From Namada tx:  
Wrapper transaction hash: 3761EDD786BBAE6D1BFA77E2F86471345F7E887C9DD816650A89D3C9E03AB0AC  
Inner transaction hash: 84B0F14784A151D0D7A06058F3BF12CD93EFB07CC9FBC67D9F264AE3476FA41B

From Osmosis tx: 3A2A387F015B53778022BFDD259352A64C0B712FC83355436F1D157D569ED31E

Link to explorer: https://www.mintscan.io/osmosis-testnet/address/osmo1e95jeru3nz4z4yz9s7va4wtc57rmgc3rrt7sep

My logs:

```
root@nmd01:~# hermes --config $HOME/.hermes/config.toml create channel --a-chain shielded-expedition.88f17d1d14 --b-chain osmo-test-5 --a-port transfer --b-port transfer --new-client-connection --yes
2024-02-25T09:53:34.139247Z INFO ThreadId(01) running Hermes v1.7.4+38f41c6
2024-02-25T09:53:34.206784Z INFO ThreadId(01) Creating new clients, new connection, and a new channel with order ORDER_UNORDERED
2024-02-25T09:53:58.204053Z INFO ThreadId(01) foreign_client.create{client=osmo-test-5->shielded-expedition.88f17d1d14:07-tendermint-0}: 🍭 client was created successfully id=07-tendermint-1482
2024-02-25T09:54:01.455079Z INFO ThreadId(01) foreign_client.create{client=shielded-expedition.88f17d1d14->osmo-test-5:07-tendermint-0}: 🍭 client was created successfully id=07-tendermint-2365
2024-02-25T09:54:20.542672Z INFO ThreadId(01) 🥂 shielded-expedition.88f17d1d14 => OpenInitConnection(OpenInit { Attributes { connection_id: connection-640, client_id: 07-tendermint-1482, counterparty_connection_id: None, counterparty_client_id: 07-tendermint-2365 } }) at height 0-62991
2024-02-25T09:54:58.376312Z INFO ThreadId(01) 🥂 osmo-test-5 => OpenTryConnection(OpenTry { Attributes { connection_id: connection-2206, client_id: 07-tendermint-2365, counterparty_connection_id: connection-640, counterparty_client_id: 07-tendermint-1482 } }) at height 5-5616847
2024-02-25T09:55:01.867553Z WARN ThreadId(01) client consensus proof height too high, waiting for destination chain to advance beyond 0-62994
2024-02-25T09:55:02.371913Z WARN ThreadId(01) client consensus proof height too high, waiting for destination chain to advance beyond 0-62994
2024-02-25T09:55:02.876194Z WARN ThreadId(01) client consensus proof height too high, waiting for destination chain to advance beyond 0-62994
2024-02-25T09:55:03.380588Z WARN ThreadId(01) client consensus proof height too high, waiting for destination chain to advance beyond 0-62994
2024-02-25T09:55:29.894701Z INFO ThreadId(01) 🥂 shielded-expedition.88f17d1d14 => OpenAckConnection(OpenAck { Attributes { connection_id: connection-640, client_id: 07-tendermint-1482, counterparty_connection_id: connection-2206, counterparty_client_id: 07-tendermint-2365 } }) at height 0-62997
2024-02-25T09:55:38.141662Z INFO ThreadId(01) 🥂 osmo-test-5 => OpenConfirmConnection(OpenConfirm { Attributes { connection_id: connection-2206, client_id: 07-tendermint-2365, counterparty_connection_id: connection-640, counterparty_client_id: 07-tendermint-1482 } }) at height 5-5616857
2024-02-25T09:55:41.195338Z INFO ThreadId(01) connection handshake already finished for Connection { delay_period: 0ns, a_side: ConnectionSide { chain: BaseChainHandle { chain_id: shielded-expedition.88f17d1d14 }, client_id: 07-tendermint-1482, connection_id: connection-640 }, b_side: ConnectionSide { chain: BaseChainHandle { chain_id: osmo-test-5 }, client_id: 07-tendermint-2365, connection_id: connection-2206 } }
2024-02-25T09:55:58.360896Z INFO ThreadId(01) 🎊 shielded-expedition.88f17d1d14 => OpenInitChannel(OpenInit { port_id: transfer, channel_id: channel-415, connection_id: None, counterparty_port_id: transfer, counterparty_channel_id: None }) at height 0-63000
2024-02-25T09:56:14.337813Z INFO ThreadId(01) 🎊 osmo-test-5 => OpenTryChannel(OpenTry { port_id: transfer, channel_id: channel-5886, connection_id: connection-2206, counterparty_port_id: transfer, counterparty_channel_id: channel-415 }) at height 5-5616866
2024-02-25T09:56:22.887676Z INFO ThreadId(01) 🎊 shielded-expedition.88f17d1d14 => OpenAckChannel(OpenAck { port_id: transfer, channel_id: channel-415, connection_id: connection-640, counterparty_port_id: transfer, counterparty_channel_id: channel-5886 }) at height 0-63003
2024-02-25T09:56:38.538368Z INFO ThreadId(01) 🎊 osmo-test-5 => OpenConfirmChannel(OpenConfirm { port_id: transfer, channel_id: channel-5886, connection_id: connection-2206, counterparty_port_id: transfer, counterparty_channel_id: channel-415 }) at height 5-5616872
2024-02-25T09:56:41.543640Z INFO ThreadId(01) channel handshake already finished for Channel { ordering: ORDER_UNORDERED, a_side: ChannelSide { chain: BaseChainHandle { chain_id: shielded-expedition.88f17d1d14 }, client_id: 07-tendermint-1482, connection_id: connection-640, port_id: transfer, channel_id: channel-415, version: None }, b_side: ChannelSide { chain: BaseChainHandle { chain_id: osmo-test-5 }, client_id: 07-tendermint-2365, connection_id: connection-2206, port_id: transfer, channel_id: channel-5886, version: None }, connection_delay: 0ns }
SUCCESS Channel {
ordering: Unordered,
a_side: ChannelSide {
chain: BaseChainHandle {
chain_id: ChainId {
id: "shielded-expedition.88f17d1d14",
version: 0,
},
runtime_sender: Sender { .. },
},
client_id: ClientId(
"07-tendermint-1482",
),
connection_id: ConnectionId(
"connection-640",
),
port_id: PortId(
"transfer",
),
channel_id: Some(
ChannelId(
"channel-415",
),
),
version: None,
},
b_side: ChannelSide {
chain: BaseChainHandle {
chain_id: ChainId {
id: "osmo-test-5",
version: 5,
},
runtime_sender: Sender { .. },
},
client_id: ClientId(
"07-tendermint-2365",
),
connection_id: ConnectionId(
"connection-2206",
),
port_id: PortId(
"transfer",
),
channel_id: Some(
ChannelId(
"channel-5886",
),
),
version: None,
},
connection_delay: 0ns,
}
```
