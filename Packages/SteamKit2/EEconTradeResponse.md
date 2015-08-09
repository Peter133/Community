You can get some information with this:

Example: 
if (EEconTradeResponse.Cancel == 0) //if the trade canceled
{
  steamFriends.SendChatMessage(callback.OtherClient, EChatEntryType.ChatMsg, "Trade Cancelled!");
  steamFriends.SetPersonaState(EPersonaState.Online);
}
if (EEconTradeResponse.Accepted == 0) //if the trade accepted
{
  steamFriends.SendChatMessage(callback.OtherClient, EChatEntryType.ChatMsg, "Trade Cancelled!");
  steamFriends.SetPersonaState(EPersonaState.Online);
}
if (EEconTradeResponse.ConnectionFailed == 0) /
{
  steamFriends.SendChatMessage(callback.OtherClient, EChatEntryType.ChatMsg, "Connection Failed");
  steamFriends.SetPersonaState(EPersonaState.Online);
}
if (EEconTradeResponse.NoResponse == 0)
{
  steamFriends.SendChatMessage(callback.OtherClient, EChatEntryType.ChatMsg, "No Response");
  steamFriends.SetPersonaState(EPersonaState.Online);
}
