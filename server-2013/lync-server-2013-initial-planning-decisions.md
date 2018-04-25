﻿---
title: 'Lync Server 2013: Decisiones de planeación iniciales'
TOCTitle: Decisiones de planeación iniciales
ms:assetid: cbaa5cb3-2b00-4b9f-952d-986a0c9f160b
ms:mtpsurl: https://technet.microsoft.com/es-es/library/Gg398855(v=OCS.15)
ms:contentKeyID: 48276701
ms.date: 01/07/2017
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Decisiones de planeación iniciales para Lync Server 2013

 

_**Última modificación del tema:** 2012-10-01_

La primera parte del proceso de planeación consiste en decidir qué cargas de trabajo y características principales de Lync Server desea para su organización.

1.  **¿Desea una implementación en línea o local?**    Lync Server admite los dos escenarios de implementación. Para obtener más información sobre cómo tomar esta decisión, vea [Decidir cómo implementar Lync Server 2013](lync-server-2013-deciding-how-to-deploy-microsoft-lync.md), anteriormente en esta sección

2.  **¿Desea una topología física o virtualizada?**    Lync Server admite todas las cargas de trabajo y roles de servidor tanto en topologías físicas como virtualizadas. La capacidad de usuarios y la escalabilidad varían entre las topologías físicas y las virtuales. Para obtener más información, vea [Ejecución de Lync Server en servidores virtuales](lync-server-2013-running-lync-server-on-virtual-servers.md).

3.  La **mensajería instantánea *(MI)* y la *presencia* siempre están habilitadas.**   En cualquier implementación de Lync Server, normalmente se instala y habilita la carga de trabajo de mensajería instantánea (MI) y presencia. La mensajería instantánea permite a los usuarios comunicarse con mensajes de texto en tiempo real y la presencia les permite ver el estado de otros usuarios en la red. El estado de presencia de un usuario proporciona información para que a los demás les sea más fácil decidir si intentan ponerse en contacto con él y de qué forma. Para obtener más información, vea [Planificar los servidores front-end, la mensajería instantánea y la presencia en Lync Server 2013](lync-server-2013-planning-for-front-end-servers-instant-messaging-and-presence.md) en la documentación de la planeación.

4.  **¿Desea implementar algún modo de conferencia?**   La conferencia es otra característica principal de Lync Server. Se admiten varios modos de conferencia. Puede elegir entre implementar todos los tipos de conferencia admitidos o solo algunos de ellos. La *conferencia web* permite a los usuarios ver un archivo, como un conjunto de diapositivas creado con el programa de gráficos de presentación Microsoft PowerPoint, que se esté presentando. El *uso compartido de aplicaciones* permite a los usuarios compartir todo su escritorio o una parte del mismo con el resto de usuarios en tiempo real. Con la *conferencia A/V*, los usuarios pueden agregar audio (y posiblemente vídeo) a sus conferencias y comunicaciones de punto a punto. La *conferencia de acceso telefónico local* permite a los usuarios usar teléfonos RTC estándar para participar en la parte de audio de conferencias hospedadas en su organización. Para obtener más información, vea [Planificar conferencias en Lync Server 2013](lync-server-2013-planning-for-conferencing.md) en la documentación sobre planeación.
    
    En Lync Server 2013, si implementa la conferencia web, también debe planear la integración con Office Web Apps Server para habilitar el uso compartido y la visualización de Powerpoint en las reuniones. Para más información, vea [Configuración de la integración de Office Web Apps Server y Lync Server 2013](lync-server-2013-enabling-office-web-apps-server-and-lync-server-2013.md).

5.  **Si implementa la característica de conferencia A/V, supervise también la calidad de audio de estas conferencias.**   Muchos factores afectan a la calidad de audio y vídeo de las conferencias A/V de Lync Server. Con la supervisión, puede supervisar la calidad de A/V de las llamadas y las conferencias. Puede detectar problemas que afectan a la calidad de medios y garantizar que los usuarios tengan la mejor experiencia de medios posible. Para obtener más información, vea [Planeamiento de la supervisión en Lync Server 2013](lync-server-2013-planning-for-monitoring.md).

6.  **¿Desea una alta disponibilidad para sus servidores de conferencia, mensajería instantánea y presencia?**   Si solo dispone de un servidor en un sitio para proporcionar las características de mensajería instantánea, presencia y conferencia, la productividad de los usuarios se verá considerablemente afectada si el servidor deja de estar disponible. Si implementa un *grupo* de Enterprise Edition de tres servidores como mínimo para estas funciones, Lync Server seguirá funcionando con todas estas características intactas aunque un servidor no esté disponible.
    
    Las organizaciones con 5.000 o menos usuarios que deseen una alta disponibilidad pueden implementar dos servidores que ejecuten Lync ServerStandard Edition y los empareje. Para obtener más información, vea [Planeación de alta disponibilidad y recuperación ante desastres en Lync Server 2013](lync-server-2013-planning-for-high-availability-and-disaster-recovery.md).

7.  **¿Quiere opciones de recuperación ante desastres?**   Si tiene dos centros de datos y desea disponer de opciones de recuperación ante desastres para que los usuarios sigan trabajando aunque todos o la mayoría de los servidores de un centro de datos dejen de funcionar, implemente los servidores teniendo en cuenta la característica de recuperación ante desastres. En esta implementación, empareje un grupo de servidores de un centro de datos con el grupo correspondiente de otro centro de datos. Si un centro de datos deja de funcionar, el otro grupo del par prestará servicio a los usuarios de los dos grupos de servidores con una interrupción mínima de los servicios. Para obtener más información, vea [Planeación de alta disponibilidad y recuperación ante desastres en Lync Server 2013](lync-server-2013-planning-for-high-availability-and-disaster-recovery.md).

8.  **¿Desea permitir a los usuarios que se comuniquen y colaboren con usuarios externos?**   Habilitar la comunicación y colaboración con usuarios externos puede aumentar el rendimiento de la inversión en Lync Server. Esto permite a los usuarios de la organización beneficiarse de características de Lync Server aunque estén trabajando fuera de los firewalls de la organización. Asimismo, puede establecer relaciones de federación con las organizaciones de socios o clientes que ejecuten Lync Server. De esta forma, los usuarios y los usuarios socios federados pueden enviar y recibir mensajes instantáneos, invitar a otros usuarios a reuniones y ver la presencia de otros usuarios con facilidad. Además, los usuarios pueden enviar un correo electrónico para invitar a usuarios externos específicos a conferencias que ellos mismos organicen. Para obtener más información, vea [Planear acceso de usuarios externos en Lync Server 2013](lync-server-2013-planning-for-external-user-access.md).

9.  **¿Desea implementar Telefonía IP empresarial?**    *Telefonía IP empresarial* es la solución de voz sobre IP (VoIP) que proporciona Lync Server. Se trata de una atractiva alternativa a la telefonía tradicional basada en PBX. La Telefonía IP empresarial permite a los usuarios realizar llamadas desde sus equipos o teléfonos VoIP haciendo clic en un contacto en Outlook o en Lync Server. Pueden realizar llamadas a través de la red IP de un PC a otro, de un PC a un teléfono o de un teléfono a un PC. Los usuarios disponen de todas las opciones de comunicación (voz, correo electrónico, mensajería instantánea y conferencia) integradas en su equipo. Para obtener más información, vea [Planear la telefonía IP empresarial en Lync Server 2013](lync-server-2013-planning-for-enterprise-voice.md) en la documentación sobre planeación.

10. **Si implementa Telefonía IP empresarial, supervise también la calidad de audio de estas llamadas.**   Recomendamos usar la supervisión para garantizar la calidad de audio de las llamadas, si implementa Telefonía IP empresarial. Para obtener más información, vea [Planeamiento de la supervisión en Lync Server 2013](lync-server-2013-planning-for-monitoring.md).

11. **¿Necesita archivar contenido de mensajería unificada o de reuniones por motivos de cumplimiento?**   Si su organización debe archivar el contenido de mensajería instantánea o de reuniones por motivos de cumplimiento, implemente un servidor de archivado. Para obtener más información, vea [Planificar el archivado en Lync Server 2013](lync-server-2013-planning-for-archiving.md).

12. **¿Desea implementar el chat persistente?**   Si desea que los usuarios tengan conversaciones en tiempo real que persistan en el tiempo, implemente el chat persistente. Para obtener más información, vea [Planeación del servidor de chat persistente en Lync Server 2013](lync-server-2013-planning-for-persistent-chat-server.md).

13. **¿Tiene Microsoft Exchange implementado?**   Si su organización usa Microsoft Exchange Server para sus servicios de correo electrónico, habilite varias características que mejoran la utilidad de Lync Server y Microsoft Exchange Server. Algunas de estas características, denominadas Mensajería unificada de Exchange (UM), habilitan a los usuarios para recibir avisos de correo de voz y escuchar correos de voz de Outlook o de Outlook Web Access, obtener acceso a sus buzones de Microsoft Exchange con un teléfono y recibir faxes en sus buzones de Microsoft Exchange. Además, si Exchange 2013 está implementado, puede integrar los almacenes de contactos para usuarios entre los dos sistemas, usar Exchange para almacenar fotos de contactos de mayor resolución e integrar el archivado de correos electrónicos y mensajes instantáneos. Para obtener más información, vea [Planificación para la integración de Exchange Server con Lync Server 2013](lync-server-2013-planning-for-exchange-server-integration.md).

14. **¿Dispone de sucursales en su organización?**   Si su organización tiene sucursales, Lync Server permite una amplia variedad de formas para admitirlas y garantizar su resistencia para características de voz, entre otras. En concreto, en una sucursal que no disponga de un vínculo WAN resistente a un centro de datos, puede instalar una Aplicación de sucursal con funciones de supervivencia o un servidor de sucursal con funciones de supervivencia para mantener la compatibilidad con Telefonía IP empresarial, en caso de que el vínculo de la red de área extensa (WAN) dejara de estar disponible. Para obtener más información, vea [Planificar la resistencia de voz en sitios de sucursal en Lync Server 2013](lync-server-2013-planning-for-branch-site-voice-resiliency.md).
