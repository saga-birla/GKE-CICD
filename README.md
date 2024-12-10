𝐀𝐮𝐭𝐨𝐦𝐚𝐭𝐢𝐧𝐠 𝐂𝐈/𝐂𝐃 𝐰𝐢𝐭𝐡 𝐆𝐨𝐨𝐠𝐥𝐞 𝐊𝐮𝐛𝐞𝐫𝐧𝐞𝐭𝐞𝐬 𝐄𝐧𝐠𝐢𝐧𝐞, 𝐂𝐥𝐨𝐮𝐝 𝐁𝐮𝐢𝐥𝐝, 𝐚𝐧𝐝 𝐂𝐥𝐨𝐮𝐝 𝐃𝐞𝐩𝐥𝐨𝐲

Today, I built a 𝗖𝗜/𝗖𝗗 𝗽𝗶𝗽𝗲𝗹𝗶𝗻𝗲 to automatically deploy applications to 𝗚𝗼𝗼𝗴𝗹𝗲 𝗞𝘂𝗯𝗲𝗿𝗻𝗲𝘁𝗲𝘀 𝗘𝗻𝗴𝗶𝗻𝗲 (𝗚𝗞𝗘) using 𝗖𝗹𝗼𝘂𝗱 𝗕𝘂𝗶𝗹𝗱 and 𝗖𝗹𝗼𝘂𝗱 𝗗𝗲𝗽𝗹𝗼𝘆! 🎉

Here’s what I did:
🔹 𝗣𝘆𝘁𝗵𝗼𝗻 𝗙𝗹𝗮𝘀𝗸 𝗔𝗽𝗽: I started by creating a simple "Hello World" Flask app, then wrote a 𝗗𝗼𝗰𝗸𝗲𝗿𝗳𝗶𝗹𝗲 to containerize it.

🔹 𝗗𝗲𝗰𝗹𝗮𝗿𝗮𝘁𝗶𝘃𝗲 𝗖𝗹𝗼𝘂𝗱 𝗗𝗲𝗽𝗹𝗼𝘆 𝗣𝗶𝗽𝗲𝗹𝗶𝗻𝗲: Instead of configuring through the console, I used a 𝗱𝗲𝗰𝗹𝗮𝗿𝗮𝘁𝗶𝘃𝗲 𝗮𝗽𝗽𝗿𝗼𝗮𝗰𝗵 with a p͟i͟p͟e͟l͟i͟n͟e͟.͟y͟a͟m͟l file. This defines two targets:

𝗗𝗲𝘃𝗲𝗹𝗼𝗽𝗺𝗲𝗻𝘁 𝗘𝗻𝘃𝗶𝗿𝗼𝗻𝗺𝗲𝗻𝘁 (𝗱𝗲𝘃.𝘆𝗮𝗺𝗹)
𝗣𝗿𝗼𝗱𝘂𝗰𝘁𝗶𝗼𝗻 𝗘𝗻𝘃𝗶𝗿𝗼𝗻𝗺𝗲𝗻𝘁 (𝗽𝗿𝗼𝗱.𝘆𝗮𝗺𝗹)
🔹 𝗞𝘂𝗯𝗲𝗿𝗻𝗲𝘁𝗲𝘀 𝗗𝗲𝗽𝗹𝗼𝘆𝗺𝗲𝗻𝘁: I wrote the YAML files to deploy the app to Kubernetes, exposing the service via a 𝗟𝗼𝗮𝗱𝗕𝗮𝗹𝗮𝗻𝗰𝗲𝗿.

🔹 𝗖𝗹𝗼𝘂𝗱 𝗕𝘂𝗶𝗹𝗱 𝗧𝗿𝗶𝗴𝗴𝗲𝗿: Configured a cloudbuild.yaml file for automatic deployment. Every time I commit changes to the GitHub repo, 𝗖𝗹𝗼𝘂𝗱 𝗕𝘂𝗶𝗹𝗱 triggers the pipeline, deploying the app to the 𝗗𝗲𝘃 𝗰𝗹𝘂𝘀𝘁𝗲𝗿 (𝘊𝘭𝘶𝘴𝘵𝘦𝘳-1). For deployment to 𝗣𝗿𝗼𝗱 𝗰𝗹𝘂𝘀𝘁𝗲𝗿 (𝘊𝘭𝘶𝘴𝘵𝘦𝘳-2), 𝗖𝗹𝗼𝘂𝗱 𝗗𝗲𝗽𝗹𝗼𝘆 requires approval before proceeding.

🔹 𝗧𝗵𝗲 𝗠𝗼𝘀𝘁 𝗖𝗵𝗮𝗹𝗹𝗲𝗻𝗴𝗶𝗻𝗴 𝗣𝗮𝗿𝘁: Writing the 𝗖𝗹𝗼𝘂𝗱 𝗗𝗲𝗽𝗹𝗼𝘆 configuration in the c͟l͟o͟u͟d͟b͟u͟i͟l͟d͟.͟y͟a͟m͟l file to create and manage 𝗱𝗲𝗽𝗹𝗼𝘆 𝗿𝗲𝗹𝗲𝗮𝘀𝗲𝘀 was the most challenging aspect of the project. It required precise configuration to automate releases and handle approvals effectively in a CI/CD environment.

This setup combines automation with controlled production releases, ensuring seamless delivery from code to clusters! 💡
