---
title: Informationen zum Windows-Subsystem für Linux
description: Erfahren Sie mehr über das Windows-Subsystem für Linux einschließlich der verschiedenen Versionen und Einsatzmöglichkeiten.
keywords: BashOnWindows, bash, wsl, windows, windowssubsystem, gnu, linux
ms.date: 07/21/2020
ms.topic: article
ms.assetid: 3cefe0db-7616-4848-a2b6-9296746a178b
ms.localizationpriority: high
ms.openlocfilehash: 0c6fa3d0c5483a7ffd1fb95f13ca62666a7c1e72
ms.sourcegitcommit: b15b847b87d29a40de4a1517315949bce9c7a3d5
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/28/2020
ms.locfileid: "91413081"
---
# <a name="what-is-the-windows-subsystem-for-linux"></a><span data-ttu-id="ef353-104">Was ist das Windows-Subsystem für Linux?</span><span class="sxs-lookup"><span data-stu-id="ef353-104">What is the Windows Subsystem for Linux?</span></span>

<span data-ttu-id="ef353-105">Mit dem Windows-Subsystem für Linux können Entwickler eine GNU-/Linux-Umgebung (einschließlich der meisten Befehlszeilentools, Hilfsprogramme und Anwendungen) direkt unter Windows unverändert ausführen, ohne den Mehraufwand eines traditionellen virtuellen Computers oder eines Dual-Boot-Setups betreiben zu müssen.</span><span class="sxs-lookup"><span data-stu-id="ef353-105">The Windows Subsystem for Linux lets developers run a GNU/Linux environment -- including most command-line tools, utilities, and applications -- directly on Windows, unmodified, without the overhead of a traditional virtual machine or dualboot setup.</span></span>

<span data-ttu-id="ef353-106">Sie haben folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="ef353-106">You can:</span></span>

* <span data-ttu-id="ef353-107">Wählen Sie Ihre bevorzugten GNU-/Linux -Distributionen aus dem [Microsoft Store](https://aka.ms/wslstore) aus.</span><span class="sxs-lookup"><span data-stu-id="ef353-107">Choose your favorite GNU/Linux distributions [from the Microsoft Store](https://aka.ms/wslstore).</span></span>
* <span data-ttu-id="ef353-108">Führen Sie gängige Befehlszeilentools wie `grep`, `sed`, `awk` oder andere ELF-64-Binärdateien aus.</span><span class="sxs-lookup"><span data-stu-id="ef353-108">Run common command-line tools such as `grep`, `sed`, `awk`, or other ELF-64 binaries.</span></span>
* <span data-ttu-id="ef353-109">Führen Sie Skripts der Bash-Shell und GNU-/Linux-Befehlszeilenanwendungen aus, beispielsweise:</span><span class="sxs-lookup"><span data-stu-id="ef353-109">Run Bash shell scripts and GNU/Linux command-line applications including:</span></span>  
    * <span data-ttu-id="ef353-110">Tools: vim, emacs, tmux</span><span class="sxs-lookup"><span data-stu-id="ef353-110">Tools: vim, emacs, tmux</span></span>
    * <span data-ttu-id="ef353-111">Sprachen: [NodeJS](/windows/nodejs/setup-on-wsl2), Javascript, [Python](/windows/python/web-frameworks), Ruby, C/C++, C# & F#, Rust, Go usw.</span><span class="sxs-lookup"><span data-stu-id="ef353-111">Languages: [NodeJS](/windows/nodejs/setup-on-wsl2), Javascript, [Python](/windows/python/web-frameworks), Ruby, C/C++, C# & F#, Rust, Go, etc.</span></span>
    * <span data-ttu-id="ef353-112">Dienste: SSHD, [MySQL](./tutorials/wsl-database.md), Apache, lighttpd, [MongoDB](./tutorials/wsl-database.md), [PostgreSQL](./tutorials/wsl-database.md).</span><span class="sxs-lookup"><span data-stu-id="ef353-112">Services: SSHD, [MySQL](./tutorials/wsl-database.md), Apache, lighttpd, [MongoDB](./tutorials/wsl-database.md), [PostgreSQL](./tutorials/wsl-database.md).</span></span>
* <span data-ttu-id="ef353-113">Installieren Sie zusätzliche Software mit Ihrem eigenen Paket-Manager für die GNU-/Linux-Distribution.</span><span class="sxs-lookup"><span data-stu-id="ef353-113">Install additional software using your own GNU/Linux distribution package manager.</span></span>
* <span data-ttu-id="ef353-114">Rufen Sie Windows-Anwendungen mithilfe einer Unix-ähnlichen Befehlszeilenshell auf.</span><span class="sxs-lookup"><span data-stu-id="ef353-114">Invoke Windows applications using a Unix-like command-line shell.</span></span>
* <span data-ttu-id="ef353-115">Rufen Sie GNU-/Linux-Anwendungen unter Windows auf.</span><span class="sxs-lookup"><span data-stu-id="ef353-115">Invoke GNU/Linux applications on Windows.</span></span>

> [!div class="nextstepaction"]
> [<span data-ttu-id="ef353-116">Installieren von WSL</span><span class="sxs-lookup"><span data-stu-id="ef353-116">Install WSL</span></span>](install-win10.md)

<br>

> [!VIDEO https://www.youtube.com/embed/48k317kOxqg]

## <a name="what-is-wsl-2"></a><span data-ttu-id="ef353-117">Was ist WSL 2?</span><span class="sxs-lookup"><span data-stu-id="ef353-117">What is WSL 2?</span></span>

<span data-ttu-id="ef353-118">WSL 2 ist eine neue Version der Windows-Subsystem für Linux-Architektur, die es dem Windows-Subsystem für Linux ermöglicht, ELF64-Linux-Binärdateien unter Windows auszuführen.</span><span class="sxs-lookup"><span data-stu-id="ef353-118">WSL 2 is a new version of the Windows Subsystem for Linux architecture that powers the Windows Subsystem for Linux to run ELF64 Linux binaries on Windows.</span></span> <span data-ttu-id="ef353-119">Die Hauptziele sind eine **gesteigerte Leistung des Dateisystems** sowie das Hinzufügen **vollständiger Kompatibilität von Systemaufrufen**.</span><span class="sxs-lookup"><span data-stu-id="ef353-119">Its primary goals are to **increase file system performance**, as well as adding **full system call compatibility**.</span></span>

<span data-ttu-id="ef353-120">Diese neue Architektur führt zu einer Änderung der Interaktion dieser Linux-Binärdateien mit Windows und der Hardware Ihres Computers, bietet aber die gleiche Benutzererfahrung wie WSL 1 (die aktuelle, allgemein verfügbar Version).</span><span class="sxs-lookup"><span data-stu-id="ef353-120">This new architecture changes how these Linux binaries interact with Windows and your computer's hardware, but still provides the same user experience as in WSL 1 (the current widely available version).</span></span>

<span data-ttu-id="ef353-121">Einzelne Linux-Verteilungen können mit der WSL 1- oder der WSL 2-Architektur ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ef353-121">Individual Linux distributions can be run with either the WSL 1 or WSL 2 architecture.</span></span> <span data-ttu-id="ef353-122">Für jede Verteilung kann jederzeit ein Upgrade oder Downgrade ausgeführt werden, und Sie können WSL 1- und WSL 2-Verteilungen parallel verwenden.</span><span class="sxs-lookup"><span data-stu-id="ef353-122">Each distribution can be upgraded or downgraded at any time and you can run WSL 1 and WSL 2 distributions side by side.</span></span> <span data-ttu-id="ef353-123">WSL 2 weist eine völlig neue Architektur auf, die von der Ausführung eines echten Linux-Kernels profitiert.</span><span class="sxs-lookup"><span data-stu-id="ef353-123">WSL 2 uses an entirely new architecture that benefits from running a real Linux kernel.</span></span>

<br>

> [!VIDEO https://www.youtube.com/embed/MrZolfGm8Zk]

## <a name="next-steps"></a><span data-ttu-id="ef353-124">Nächste Schritte</span><span class="sxs-lookup"><span data-stu-id="ef353-124">Next steps</span></span>

* [<span data-ttu-id="ef353-125">Installieren von WSL 1 und Aktualisieren auf WSL 2</span><span class="sxs-lookup"><span data-stu-id="ef353-125">Install WSL 1 and update to WSL 2</span></span>](./install-win10.md)

* [<span data-ttu-id="ef353-126">Vergleich zwischen WSL 2 und WSL 1</span><span class="sxs-lookup"><span data-stu-id="ef353-126">Compare WSL 2 and WSL 1</span></span>](./compare-versions.md)

* [<span data-ttu-id="ef353-127">Erstellen eines Benutzerkontos und Kennworts für Ihre neue Linux-Verteilung</span><span class="sxs-lookup"><span data-stu-id="ef353-127">Create a user account and password for your new Linux distribution</span></span>](./user-support.md)

* [<span data-ttu-id="ef353-128">Häufig gestellte Fragen (FAQ)</span><span class="sxs-lookup"><span data-stu-id="ef353-128">Read Frequently Asked Questions</span></span>](./faq.md)

* [<span data-ttu-id="ef353-129">Häufig gestellte Fragen zu WSL 2</span><span class="sxs-lookup"><span data-stu-id="ef353-129">Read Frequently Asked Questions about WSL 2</span></span>](./wsl2-faq.md)

* [<span data-ttu-id="ef353-130">Problembehandlung</span><span class="sxs-lookup"><span data-stu-id="ef353-130">Troubleshooting</span></span>](./troubleshooting.md)

* [<span data-ttu-id="ef353-131">Ausführen von Interoperabilitätsbefehlen zwischen Windows und Linux</span><span class="sxs-lookup"><span data-stu-id="ef353-131">Run interoperability commands between Windows and Linux</span></span>](./interop.md)

* [<span data-ttu-id="ef353-132">Ausführen von Startbefehlen und Konfigurationen</span><span class="sxs-lookup"><span data-stu-id="ef353-132">Run launch commands and configurations</span></span>](./wsl-config.md)

* [<span data-ttu-id="ef353-133">Einrichten von Dateiberechtigungen</span><span class="sxs-lookup"><span data-stu-id="ef353-133">Set up file permissions</span></span>](./file-permissions.md)

* [<span data-ttu-id="ef353-134">Einrichten von WSL für Unternehmen</span><span class="sxs-lookup"><span data-stu-id="ef353-134">Set up WSL for Enterprise</span></span>](./enterprise.md)

* [<span data-ttu-id="ef353-135">Verweisen auf WSL-Befehle</span><span class="sxs-lookup"><span data-stu-id="ef353-135">Reference WSL commands</span></span>](./reference.md)

* [<span data-ttu-id="ef353-136">Erstellen von benutzerdefinierten Verteilungen</span><span class="sxs-lookup"><span data-stu-id="ef353-136">Build custom distributions</span></span>](./build-custom-distro.md)

* [<span data-ttu-id="ef353-137">Lesen Sie die Anmerkungen zu dieser Version von WSL.</span><span class="sxs-lookup"><span data-stu-id="ef353-137">Read the WSL Release Notes</span></span>](./release-notes.md)