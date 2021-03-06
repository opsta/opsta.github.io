---
layout: post
title: "สรุป Highlight จากงาน GDG Cloud Bangkok 1st Meetup"
author_github: mrnonz
date: 2017-09-29 13:14:15 +0700
categories: meetup
image: /assets/20170929/small-banner-gdg-cloud-bangkok.jpg
fbcomments: yes
---

![GDG Cloud Bangkok Banner]({{ site.url }}/assets/20170929/small-banner-gdg-cloud-bangkok.jpg){: .center-image }

# GDG Cloud Bangkok 1st Meetup.

สำหรับใครที่ไม่ได้มาร่วมงาน หรืออยากอ่านสรุปย้อนหลังตามได้จากที่นี่เลยครับ

งาน GDG Cloud Bangkok 1st Meetup ครั้งนี้ถูกจัดขึ้นที่ Google Office Thailand ที่อาคาร Park Ventures ชั้น 16 แถวๆ BTS เพลินจิตนี่เอง ถึงแม้ชื่องานจะเป็นจังหวัดกรุงเทพมหานคร แต่เราเปิดรับผู้เข้าร่วมงานจากทุกจังหวัดแน่นอนครับ

<!--more-->

---

## "Introduction to Google Cloud" by Paiboon Wongsasutthikul

![Paiboon Present]({{ site.url }}/assets/20170929/paiboon-present.jpg){: .center-image }

คุณ **[Paiboon Wongsasutthikul][Linkedin-Paiboon]** Territory Lead, Google Cloud Thailand ได้เล่าความเป็นมาของ Google โดยแบ่งยุคของโลกไอทีเป็น 3 ส่วน
1. ยุค Web 1990's
2. ยุค Mobile 2000's
3. ยุคปัจจุบัน Internet of things & Smarter (AI) โดยมีคำกล่าวของคุณ Sundar Pichai, Google CEO คนปัจจุบันว่า

> ### *We will move from mobile first to an AI first world.*

Google Cloud เริ่มจากตั้งแต่ Infrastructure ขึ้นไปจนถึงการทำ SaaS กว่าจะมาเป็น Google Cloud ที่มีความเสถียรสูงขนาดนี้ โดยถูกหล่อหลอมมาจากประสบการณ์ และความเจ็บปวดที่มากมายจากโลกแห่งความเป็นจริงของ Google เอง

Spotify, Traveloka, Carousell, Omise เป็นหนึ่งในความไว้วางใจที่เลือกใช้ Google Cloud ให้เป็นผู้ดูแลส่วนนี้ด้วย

---

## "Where Should I Run My Code?” by Richard Coombes

![GCP Summary]({{ site.url }}/assets/20170929/gcp-summary.svg){: .center-image }

คุณ **[Richard Coombes][Linkedin-Richard]** Customer Engineer จาก Google ได้พาเราไปเจาะลึกกับเรื่องราวเกี่ยวกับ Google Cloud Platform (GCP) ว่ามีของเด็ดอะไรบ้าง รวมไปถึงมีการสาธิตการใช้งานให้ดูในงานกันเลยทีเดียว

* **Compute Engine (GCE)** คุณสามารถเลือก Spec ที่เหมาะสมกับคุณได้ทันที รวมไปถึงการ Scale ก็สามารถทำได้อย่างง่ายดาย รวมไปถึงหากคุณใช้ Spec ที่สูงเกินความจำเป็นทาง GCP เองก็มีแจ้งเตือนว่าเราสามารถลด Spec เพื่อประหยัดเงินในส่วนนั้นๆ ได้ด้วย
* **Container Engine (GKE)** จากประโยคที่ว่า

  > ### *Manage applications, not machines.*

  GKE คือ Service ที่ทำให้เราสามารถรัน Container จากตัว Image ของเราขึ้นมาได้ทันที โดยไม่ต้องสร้าง Server ขึ้นมาเอง และเครื่องมือที่กำลังมาแรงในตอนนี้นั้นก็คือ [Kubernetes (k8s)][Kubernetes] ที่ถือเป็น open-source อย่าง 100% โดย k8s ทำให้เราสามารถจัดการกับ Container ต่างๆ ที่ง่ายยิ่งขึ้น ไม่ว่าจะเป็นการทำ Auto-Deploy, Scaling, Manage Container เป็นต้น
* **App Engine (GAE)** ที่ทำให้เราสามารถใช้งาน App ได้โดยไม่ต้องมาสร้าง Infrastructure เอง เพียงแค่ส่ง Code ของเราขึ้นไปให้ GCP จัดการก็สามารถใช้งานได้เลย ภาษาที่ใช้งานได้ในตอนนี้ คือ  Node.js, Java, Ruby, C#, Go, Python,PHP และ **.NET** ที่สำคัญหากภาษาไหนไม่รองรับ เราสามารถนำ Docker ขึ้นไปรันบน App Engine ภายใต้ชื่อของ **App Engine Flexible Environment** ได้อีกด้วย
* **Cloud Functions (BETA)** คือ Serverless ที่ทำให้เราสามารถใช้งานฟังก์ชันใดๆ ก็ได้ของเรา โดยไม่ได้มีการสร้าง Server รอไว้ แต่จะสามารถทำงานได้ทันทีเมื่อถูกเรียกใช้งานเลย
* **Load Balancing** ฟีเจอร์ที่ถือว่าเป็น Highlight ของ Load balancing คือ เราสามารถ Specific ได้ว่าจะให้ Traffic ที่เข้ามานั้นวิ่งไปยังที่ไหนปลายทางตาม %, IP, Random รวมไปถึงมีการป้องกัน DDoS ให้เราระดับนึงอีกด้วย (คุณ Paiboon แอบบอกว่า [google.com][Google] ก็ใช้ตัวนี้เหมือนกันครับ ไว้ใจได้แน่นอน)

---

## "Jitta Case Study" by Sila Sujjinanont

![Jitta Present]({{ site.url }}/assets/20170929/Jitta-highres.jpeg){: .center-image }

คุณ **[Sila Sujjinanont][Linkedin-Sila]** Head of Infrastructure and Security จาก [Jitta.com][Jitta] ได้มาบอกกล่าวถึงประสบการณ์มากกว่า 2 ปีกับ Kubernetes ว่าทั้งมีความสุข และพบปัญหาอะไรบ้าง

> ### *Great Infrastructure = Development Speed + More Creative + More Growth*

* **ความเจ็บปวด** คุณ Sila เล่าให้ฟังว่า Jitta เริ่มจากการสร้างสิ่งที่เหมือนกันกับ Kubernetes ขึ้นมาเพื่อใช้งานเองตั้งแต่ 2 ปีก่อน โดยเครื่องมือนี้สามารถทำได้ตั้งแต่การกดปุ่มเพื่อสร้าง Instance ขึ้นมาเลยทีเดียว รวมไปถึงการ SSH-Server จากหน้าเว็บไซต์ ซึ่งถือเป็นความเจ็บปวดอย่างมาก เพราะต้องเสียกำลังคนไปกับการดูแลส่วนนี้ถึง 2 คน ยังไม่รวมไปถึงกับ Bug ที่มากมายตามสิ่งที่สร้างขึ้นมา เพราะเป็นเครื่องมือที่ยิ่งใหญ่มาก
* **ทางเลือกใหม่กับ Kubernetes** ทาง Jitta ทดสอบการทำงานของอย่างหนักมาก เพื่อความมั่นใจสำหรับทางเลือกใหม่ ตั้งแต่การทดลองปิด Node ทิ้งเพื่อทดสอบความสามารถในการ Recovery รวมไปถึงเป้าหมายระยะยาวของ k8s เอง ว่ามีกลุ่มหรือองค์กรใดสนับสนุนแค่ไหน
* **Log & Monitoring** คุณ Sila เน้นย้ำมากว่าการทำ Log และ Monitor ถือเป็นสิ่งที่สำคัญอย่างมาก ทุกคนควรที่จะทำ และทาง Jitta เองทำส่วนนี้ไว้อย่างดีมาก จึงพบปัญหาก่อนเกิดเหตุการณ์ไม่คาดฝัน รวมไปถึงการทำ Manual Test ด้วยการสุ่มปิด Node ทิ้งดื้อๆ โดยเป็นวิธีเดียวกันกับทาง Netflix เองก็ใช้อยู่เช่นกัน
* **DDoS** เป็นอีกหนึ่งเสียงที่ยืนยันว่าทาง Google Load Balancing ช่วยป้องกัน DDoS ระดับนึง เพราะทาง Jitta เองก็เคยโดน DDoS มาบ้างเช่นกัน

---

หากท่านใดสนใจดูการถ่ายทอดสดย้อนหลัง สามารถดูได้ที่นี่เลยครับ [GDG Cloud Bangkok FB Live][GDG-Cloud-Bangkok-FBLive]

หากใครพลาดงานนี้ สามารถรอติดตามงาน Meetup ครั้งต่อไปของกลุ่ม GDG Cloud Bangkok ได้โดยการ [Join Facebook Group][Join-Facebook-Group] เพื่อรับข่าวสารไว้ได้เลย แล้วพบกันในงานถัดไปนะครับ

ขอบคุณครับ

![GDG Meetup Group Shot]({{ site.url }}/assets/20170929/gdg-group-shot-highres.jpeg){: .center-image }

[Join-Facebook-Group]: https://www.facebook.com/groups/115166445851226/
[Google]: https://www.google.com/
[Linkedin-Paiboon]: https://www.linkedin.com/in/meetpaiboon/
[Linkedin-Richard]: https://www.linkedin.com/in/coombesr
[Linkedin-Sila]: https://www.linkedin.com/in/silasujjinanont/
[Kubernetes]: https://kubernetes.io/
[Jitta]: https://www.jitta.com/
[GDG-Cloud-Bangkok-FBLive]: https://www.facebook.com/GDG-Cloud-Bangkok-FB-Live-795562247271667/
