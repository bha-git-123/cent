def attachments = [
  [
    text: 'Jenkins testing',
    fallback: 'Hey, Vader seems to be mad at you.',
    color: 'good'
  ]
]
node {
  sh "echo hey > blah.txt"
  slackSend(channel: '#mcms-iscp-developer', attachments: attachments)
  slackUploadFile channel: "#mcms-iscp-developer", filePath: "blah.txt", initialComment:  'HEY HEY'
}


