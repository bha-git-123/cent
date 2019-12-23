def attachments = [
  [
    text: 'Jenkins testing',
    fallback: 'Hey, Vader seems to be mad at you.',
    color: 'good'
  ]
]
node {
  sh "echo hey > blah.txt"
  slackSend(channel: '#automation', attachments: attachments)
  slackUploadFile channel: "#automation", filePath: "blah.txt", initialComment:  'HEY HEY'
}


