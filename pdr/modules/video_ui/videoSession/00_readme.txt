Fichiers pour process puredata dédié au traitement vidéo 
	ce module communiquera par local network avec un process puredata audio 
	(session PdRacks) contenant les modules de l'extension video_ui

Liste des fichiers dans ce répertoire

-videoSession2.pd
	module communiquant avec les modules compatibles PdRacks de l'extension video_ui
		data_upic
		data_feuille
		data_cyclogroove

-videoSessionPSM  
	semblable à videoSession2 avec la prise en charge des points convexity en plus

-video.pd
	contient videoSession2 et le connecte à pix_video
-video_openni.pd
	contient videoSession2 et le connecte à pix_openni (testé sous Windows)

-ofelia_Session
	semblable au module data_ofelia, mais prévu pour fonctionner dans une 
	session puredata distincte, qui se connectera via local network à une 
	autre session pd audio PdRacks contenant le module data_cyclogroove