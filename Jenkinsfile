def attachments = [
  [
    text: 'Jenkins testing is going on',
    fallback: 'Hey, Vader seems to be mad at you.',
    color: '#ff0000'
  ]
]
node {
  sh "echo hey > blah.txt"
  slackUploadFile filePath: '*.txt', initialComment:  'HEY HEY'
}

slackSend(channel: '#mcms-iscp-developer', attachments: attachments)
