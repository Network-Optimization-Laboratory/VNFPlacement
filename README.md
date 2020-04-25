# VNFPlacement
java -jar -Dapp.home="[ubicacionDelClonado]/VNFPlacement/src/main/resources/" [ubicacionJar]/[nombreJar].jar

Valores Iniciales
2020-04-25 17:23:43,210 [main           ] INFO  DataService                    - Valores iniciales: 
2020-04-25 17:23:43,212 [main           ] INFO  DataService                    - VNFs: 
2020-04-25 17:23:43,231 [main           ] INFO  DataService                    - Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}
2020-04-25 17:23:43,232 [main           ] INFO  DataService                    - Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}
2020-04-25 17:23:43,232 [main           ] INFO  DataService                    - Vnf{id='Proxy', delay=5, deploy=25, resourceCPU=4, resourceRAM=3, resourceStorage=8, licenceCost=85.0, bandwidthFactor=0.5}
2020-04-25 17:23:43,233 [main           ] INFO  DataService                    - Vnf{id='NAT', delay=8, deploy=10, resourceCPU=5, resourceRAM=4, resourceStorage=10, licenceCost=60.0, bandwidthFactor=0.7}
2020-04-25 17:23:43,233 [main           ] INFO  DataService                    - Vnf{id='DPI', delay=10, deploy=50, resourceCPU=2, resourceRAM=2, resourceStorage=5, licenceCost=90.0, bandwidthFactor=1.2}
2020-04-25 17:23:43,233 [main           ] INFO  DataService                    - Servidores: 
2020-04-25 17:23:43,241 [main           ] INFO  DataService                    - Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}
2020-04-25 17:23:43,242 [main           ] INFO  DataService                    - Server{id='server2', vnf=[], licenceCost=100.0, energyCost=0.2, resourceCPU=14, resourceRAM=6, resourceStorage=120, resourceCPUCost=5.0, resourceRAMCost=2.0, resourceStorageCost=2.5, energyPerCoreWatts=85, energyPeakWatts=3000, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}
2020-04-25 17:23:43,243 [main           ] INFO  DataService                    - Server{id='server3', vnf=[], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}
2020-04-25 17:23:43,243 [main           ] INFO  DataService                    - Nodos: 
2020-04-25 17:23:43,248 [main           ] INFO  DataService                    - Node:id='node1', server=null, energyCost=0.7
2020-04-25 17:23:43,249 [main           ] INFO  DataService                    - Node:id='node2', server=Server{id='server2', vnf=[], licenceCost=100.0, energyCost=0.2, resourceCPU=14, resourceRAM=6, resourceStorage=120, resourceCPUCost=5.0, resourceRAMCost=2.0, resourceStorageCost=2.5, energyPerCoreWatts=85, energyPeakWatts=3000, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.5
2020-04-25 17:23:43,249 [main           ] INFO  DataService                    - Node:id='node3', server=Server{id='server3', vnf=[], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.4
2020-04-25 17:23:43,249 [main           ] INFO  DataService                    - Node:id='node4', server=Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.3
2020-04-25 17:23:43,250 [main           ] INFO  DataService                    - Node:id='node5', server=null, energyCost=0.6
2020-04-25 17:23:43,250 [main           ] INFO  DataService                    - Node:id='node6', server=null, energyCost=0.2
2020-04-25 17:23:43,250 [main           ] INFO  DataService                    - Matrices: 
2020-04-25 17:23:43,252 [main           ] INFO  DataService                    - Cantidad de nodos: 6
2020-04-25 17:23:43,252 [main           ] INFO  DataService                    - Matriz Nodos
2020-04-25 17:23:43,253 [main           ] INFO  DataService                    - [[0, 1, 0, 1, 0, 0], [0, 0, 1, 1, 0, 0], [0, 0, 0, 0, 1, 0], [0, 0, 1, 0, 1, 0], [0, 0, 0, 0, 0, 1], [0, 0, 0, 0, 0, 0]]
2020-04-25 17:23:43,253 [main           ] INFO  DataService                    - Matriz de Delay
2020-04-25 17:23:43,255 [main           ] INFO  DataService                    - [[0, 2, 0, 3, 0, 0], [0, 0, 4, 3, 0, 0], [0, 0, 0, 0, 2, 0], [0, 0, 5, 0, 3, 0], [0, 0, 0, 0, 0, 5], [0, 0, 0, 0, 0, 0]]
2020-04-25 17:23:43,255 [main           ] INFO  DataService                    - Matriz de Distancia
2020-04-25 17:23:43,261 [main           ] INFO  DataService                    - [[0, 80, 0, 60, 0, 0], [0, 0, 75, 70, 0, 0], [0, 0, 0, 0, 100, 0], [0, 0, 55, 0, 120, 0], [0, 0, 0, 0, 0, 97], [0, 0, 0, 0, 0, 0]]
2020-04-25 17:23:43,261 [main           ] INFO  DataService                    - Matriz de Ancho de Banda
2020-04-25 17:23:43,266 [main           ] INFO  DataService                    - [[0.0, 800.0, 0.0, 900.0, 0.0, 0.0], [0.0, 0.0, 700.0, 600.0, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0, 650.0, 0.0], [0.0, 0.0, 500.0, 0.0, 750.0, 0.0], [0.0, 0.0, 0.0, 0.0, 0.0, 970.0], [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]]
2020-04-25 17:23:43,267 [main           ] INFO  DataService                    - Matriz de costo por unidad de Mbit
2020-04-25 17:23:43,272 [main           ] INFO  DataService                    - [[0.0, 0.3, 0.0, 0.2, 0.0, 0.0], [0.0, 0.0, 0.4, 0.3, 0.0, 0.0], [0.0, 0.0, 0.0, 0.0, 0.5, 0.0], [0.0, 0.0, 0.5, 0.0, 0.4, 0.0], [0.0, 0.0, 0.0, 0.0, 0.0, 0.2], [0.0, 0.0, 0.0, 0.0, 0.0, 0.0]]
2020-04-25 17:23:43,274 [main           ] INFO  DataService                    - Enlaces: 
2020-04-25 17:23:43,278 [main           ] INFO  DataService                    - Link{id='node1-node2', delay=2, distance=80, bandwidth=800.0, bandwidthCost=0.3, bandwidthUsed=0.0}
2020-04-25 17:23:43,297 [main           ] INFO  DataService                    - Link{id='node1-node4', delay=3, distance=60, bandwidth=900.0, bandwidthCost=0.2, bandwidthUsed=0.0}
2020-04-25 17:23:43,298 [main           ] INFO  DataService                    - Link{id='node2-node3', delay=4, distance=75, bandwidth=700.0, bandwidthCost=0.4, bandwidthUsed=0.0}
2020-04-25 17:23:43,303 [main           ] INFO  DataService                    - Link{id='node2-node4', delay=3, distance=70, bandwidth=600.0, bandwidthCost=0.3, bandwidthUsed=0.0}
2020-04-25 17:23:43,305 [main           ] INFO  DataService                    - Link{id='node3-node5', delay=2, distance=100, bandwidth=650.0, bandwidthCost=0.5, bandwidthUsed=0.0}
2020-04-25 17:23:43,309 [main           ] INFO  DataService                    - Link{id='node4-node3', delay=5, distance=55, bandwidth=500.0, bandwidthCost=0.5, bandwidthUsed=0.0}
2020-04-25 17:23:43,310 [main           ] INFO  DataService                    - Link{id='node4-node5', delay=3, distance=120, bandwidth=750.0, bandwidthCost=0.4, bandwidthUsed=0.0}
2020-04-25 17:23:43,310 [main           ] INFO  DataService                    - Link{id='node5-node6', delay=5, distance=97, bandwidth=970.0, bandwidthCost=0.2, bandwidthUsed=0.0}
2020-04-25 17:23:43,311 [main           ] INFO  DataService                    - Grafo: 
2020-04-25 17:23:43,323 [main           ] INFO  DataService                    - ([Node:id='node1', server=null, energyCost=0.7, Node:id='node2', server=Server{id='server2', vnf=[], licenceCost=100.0, energyCost=0.2, resourceCPU=14, resourceRAM=6, resourceStorage=120, resourceCPUCost=5.0, resourceRAMCost=2.0, resourceStorageCost=2.5, energyPerCoreWatts=85, energyPeakWatts=3000, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.5, Node:id='node3', server=Server{id='server3', vnf=[], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.4, Node:id='node4', server=Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.3, Node:id='node5', server=null, energyCost=0.6, Node:id='node6', server=null, energyCost=0.2], [Link{id='node1-node2', delay=2, distance=80, bandwidth=800.0, bandwidthCost=0.3, bandwidthUsed=0.0}=(Node:id='node1', server=null, energyCost=0.7,Node:id='node2', server=Server{id='server2', vnf=[], licenceCost=100.0, energyCost=0.2, resourceCPU=14, resourceRAM=6, resourceStorage=120, resourceCPUCost=5.0, resourceRAMCost=2.0, resourceStorageCost=2.5, energyPerCoreWatts=85, energyPeakWatts=3000, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.5), Link{id='node1-node4', delay=3, distance=60, bandwidth=900.0, bandwidthCost=0.2, bandwidthUsed=0.0}=(Node:id='node1', server=null, energyCost=0.7,Node:id='node4', server=Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.3), Link{id='node2-node3', delay=4, distance=75, bandwidth=700.0, bandwidthCost=0.4, bandwidthUsed=0.0}=(Node:id='node2', server=Server{id='server2', vnf=[], licenceCost=100.0, energyCost=0.2, resourceCPU=14, resourceRAM=6, resourceStorage=120, resourceCPUCost=5.0, resourceRAMCost=2.0, resourceStorageCost=2.5, energyPerCoreWatts=85, energyPeakWatts=3000, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.5,Node:id='node3', server=Server{id='server3', vnf=[], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.4), Link{id='node2-node4', delay=3, distance=70, bandwidth=600.0, bandwidthCost=0.3, bandwidthUsed=0.0}=(Node:id='node2', server=Server{id='server2', vnf=[], licenceCost=100.0, energyCost=0.2, resourceCPU=14, resourceRAM=6, resourceStorage=120, resourceCPUCost=5.0, resourceRAMCost=2.0, resourceStorageCost=2.5, energyPerCoreWatts=85, energyPeakWatts=3000, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.5,Node:id='node4', server=Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.3), Link{id='node3-node5', delay=2, distance=100, bandwidth=650.0, bandwidthCost=0.5, bandwidthUsed=0.0}=(Node:id='node3', server=Server{id='server3', vnf=[], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.4,Node:id='node5', server=null, energyCost=0.6), Link{id='node4-node3', delay=5, distance=55, bandwidth=500.0, bandwidthCost=0.5, bandwidthUsed=0.0}=(Node:id='node4', server=Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.3,Node:id='node3', server=Server{id='server3', vnf=[], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.4), Link{id='node4-node5', delay=3, distance=120, bandwidth=750.0, bandwidthCost=0.4, bandwidthUsed=0.0}=(Node:id='node4', server=Server{id='server1', vnf=[], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=0, resourceStorageUsed=0, resourceCPUUsed=0, energyUsed=0}, energyCost=0.3,Node:id='node5', server=null, energyCost=0.6), Link{id='node5-node6', delay=5, distance=97, bandwidth=970.0, bandwidthCost=0.2, bandwidthUsed=0.0}=(Node:id='node5', server=null, energyCost=0.6,Node:id='node6', server=null, energyCost=0.2)])

Solucion 1
2020-04-25 17:39:43,370 [main           ] INFO  VnfService                     - Valores de la Solucion
2020-04-25 17:23:43,378 [main           ] INFO  VnfService                     - Trafico: 
2020-04-25 17:23:43,378 [main           ] INFO  VnfService                     - Traffic: nodeOrigin=node1, nodeDestiny=node6, bandwidth=183, delayMaxSLA=24, penaltyCostSLO=2.0, sfc=SFC{vnfs=[Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}, Vnf{id='Proxy', delay=5, deploy=25, resourceCPU=4, resourceRAM=3, resourceStorage=8, licenceCost=85.0, bandwidthFactor=0.5}, Vnf{id='NAT', delay=8, deploy=10, resourceCPU=5, resourceRAM=4, resourceStorage=10, licenceCost=60.0, bandwidthFactor=0.7}]}
2020-04-25 17:23:43,379 [main           ] INFO  VnfService                     - Nodos de las Solucion: 
2020-04-25 17:23:43,379 [main           ] INFO  VnfService                     - Node:id='node1', server=null, energyCost=0.7
2020-04-25 17:23:43,379 [main           ] INFO  VnfService                     - Node:id='node4', server=Server{id='server1', vnf=[Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}, Vnf{id='Proxy', delay=5, deploy=25, resourceCPU=4, resourceRAM=3, resourceStorage=8, licenceCost=85.0, bandwidthFactor=0.5}], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=7, resourceStorageUsed=14, resourceCPUUsed=7, energyUsed=560}, energyCost=0.3
2020-04-25 17:23:43,379 [main           ] INFO  VnfService                     - Node:id='node3', server=Server{id='server3', vnf=[Vnf{id='NAT', delay=8, deploy=10, resourceCPU=5, resourceRAM=4, resourceStorage=10, licenceCost=60.0, bandwidthFactor=0.7}], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=4, resourceStorageUsed=10, resourceCPUUsed=5, energyUsed=350}, energyCost=0.4
2020-04-25 17:23:43,380 [main           ] INFO  VnfService                     - Node:id='node5', server=null, energyCost=0.6
2020-04-25 17:23:43,380 [main           ] INFO  VnfService                     - Node:id='node6', server=null, energyCost=0.2
2020-04-25 17:23:43,380 [main           ] INFO  VnfService                     - Enlace de la Solucion: 
2020-04-25 17:23:43,380 [main           ] INFO  VnfService                     - Link{id='node1-node4', delay=3, distance=60, bandwidth=900.0, bandwidthCost=0.2, bandwidthUsed=183.0}
2020-04-25 17:23:43,380 [main           ] INFO  VnfService                     - Link{id='node4-node3', delay=5, distance=55, bandwidth=500.0, bandwidthCost=0.5, bandwidthUsed=73.2}
2020-04-25 17:23:43,380 [main           ] INFO  VnfService                     - Link{id='node3-node5', delay=2, distance=100, bandwidth=650.0, bandwidthCost=0.5, bandwidthUsed=51.24}
2020-04-25 17:23:43,381 [main           ] INFO  VnfService                     - Link{id='node5-node6', delay=5, distance=97, bandwidth=970.0, bandwidthCost=0.2, bandwidthUsed=51.24}

2020-04-25 17:23:43,381 [main           ] INFO  VnfService                     - Funciones Objetivos con sus resultados: 
2020-04-25 17:23:43,381 [main           ] INFO  VnfService                     - Costo de Energia total: 145.7
2020-04-25 17:23:43,381 [main           ] INFO  VnfService                     - Costo de Reenvio de Trafico: 254.76799999999997
2020-04-25 17:23:43,381 [main           ] INFO  VnfService                     - Cantidad de Hosts o Servidores utilizados: 2
2020-04-25 17:23:43,381 [main           ] INFO  VnfService                     - Costo de latencia/Retardo/Retraso total: 32
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Costo de Instalacion o Configuracion total: 55
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Distancia total: 312
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Numero de Saltos/Numero de enlaces de la ruta: 4
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Ancho de banda total: 358.68
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Numero de instancias: 3
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Trafico de Carga: 11477.76
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Recursos total:137.8
2020-04-25 17:23:43,382 [main           ] INFO  VnfService                     - Costo por SLO: 2.0
2020-04-25 17:23:43,383 [main           ] INFO  VnfService                     - Costo de licencia total: 400.0
2020-04-25 17:23:43,383 [main           ] INFO  VnfService                     - Costo de Fragmentacion: 108.7996
2020-04-25 17:23:43,383 [main           ] INFO  VnfService                     - Costo de todos los enlaces: 109.06800000000001
2020-04-25 17:23:43,405 [main           ] INFO  VnfService                     - Maxima uitlizacion del enlace: 183.0


Solucion 2
2020-04-25 17:39:17,970 [main           ] INFO  VnfService                     - Valores de la Solucion
2020-04-25 17:38:17,975 [main           ] INFO  VnfService                     - Trafico: 
2020-04-25 17:38:17,975 [main           ] INFO  VnfService                     - Traffic: nodeOrigin=node1, nodeDestiny=node6, bandwidth=170, delayMaxSLA=12, penaltyCostSLO=1.0, sfc=SFC{vnfs=[Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}, Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}, Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}]}
2020-04-25 17:38:17,976 [main           ] INFO  VnfService                     - Nodos de las Solucion: 
2020-04-25 17:38:17,976 [main           ] INFO  VnfService                     - Node:id='node1', server=null, energyCost=0.7
2020-04-25 17:38:17,976 [main           ] INFO  VnfService                     - Node:id='node4', server=Server{id='server1', vnf=[Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=2, resourceStorageUsed=9, resourceCPUUsed=3, energyUsed=240}, energyCost=0.3
2020-04-25 17:38:17,977 [main           ] INFO  VnfService                     - Node:id='node3', server=Server{id='server3', vnf=[Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}, Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=6, resourceStorageUsed=15, resourceCPUUsed=6, energyUsed=420}, energyCost=0.4
2020-04-25 17:38:17,977 [main           ] INFO  VnfService                     - Node:id='node5', server=null, energyCost=0.6
2020-04-25 17:38:17,977 [main           ] INFO  VnfService                     - Node:id='node6', server=null, energyCost=0.2
2020-04-25 17:38:17,977 [main           ] INFO  VnfService                     - Enlaces de la Solucion: 
2020-04-25 17:38:17,977 [main           ] INFO  VnfService                     - Link{id='node1-node4', delay=3, distance=60, bandwidth=900.0, bandwidthCost=0.2, bandwidthUsed=170.0}
2020-04-25 17:38:17,978 [main           ] INFO  VnfService                     - Link{id='node4-node3', delay=5, distance=55, bandwidth=500.0, bandwidthCost=0.5, bandwidthUsed=153.0}
2020-04-25 17:38:17,978 [main           ] INFO  VnfService                     - Link{id='node3-node5', delay=2, distance=100, bandwidth=650.0, bandwidthCost=0.5, bandwidthUsed=110.16000000000001}
2020-04-25 17:38:17,978 [main           ] INFO  VnfService                     - Link{id='node5-node6', delay=5, distance=97, bandwidth=970.0, bandwidthCost=0.2, bandwidthUsed=110.16000000000001}

2020-04-25 17:38:17,978 [main           ] INFO  VnfService                     - Funciones Objetivos con sus resultados: 
2020-04-25 17:38:17,979 [main           ] INFO  VnfService                     - Costo de Energia total: 131.2
2020-04-25 17:38:17,979 [main           ] INFO  VnfService                     - Costo de Reenvio de Trafico: 318.81199999999995
2020-04-25 17:38:17,979 [main           ] INFO  VnfService                     - Cantidad de Hosts o Servidores utilizados: 2
2020-04-25 17:38:17,979 [main           ] INFO  VnfService                     - Costo de latencia/Retardo/Retraso total: 43
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Costo de Instalacion o Configuracion total: 80
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Distancia total: 312
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Numero de Saltos/Numero de enlaces de la ruta: 4
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Ancho de banda total: 543.32
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Numero de instancias: 3
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Trafico de Carga: 23362.760000000002
2020-04-25 17:38:17,980 [main           ] INFO  VnfService                     - Recursos total:114.3
2020-04-25 17:38:17,981 [main           ] INFO  VnfService                     - Costo por SLO: 1.0
2020-04-25 17:38:17,981 [main           ] INFO  VnfService                     - Costo de licencia total: 415.0
2020-04-25 17:38:17,981 [main           ] INFO  VnfService                     - Costo de Fragmentacion: 103.35040000000001
2020-04-25 17:38:17,981 [main           ] INFO  VnfService                     - Costo de todos los enlaces: 187.61200000000002
2020-04-25 17:38:17,988 [main           ] INFO  VnfService                     - Maxima uitlizacion del enlace: 170.0


Solucion 3
2020-04-25 17:39:12,006 [main           ] INFO  VnfService                     - Valores de la Solucion
2020-04-25 17:39:12,007 [main           ] INFO  VnfService                     - Trafico: 
2020-04-25 17:39:12,007 [main           ] INFO  VnfService                     - Traffic: nodeOrigin=node1, nodeDestiny=node6, bandwidth=294, delayMaxSLA=23, penaltyCostSLO=3.0, sfc=SFC{vnfs=[Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}, Vnf{id='Proxy', delay=5, deploy=25, resourceCPU=4, resourceRAM=3, resourceStorage=8, licenceCost=85.0, bandwidthFactor=0.5}, Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}]}
2020-04-25 17:39:12,008 [main           ] INFO  VnfService                     - Nodos de las Solucion: 
2020-04-25 17:39:12,008 [main           ] INFO  VnfService                     - Node:id='node1', server=null, energyCost=0.7
2020-04-25 17:39:12,008 [main           ] INFO  VnfService                     - Node:id='node4', server=Server{id='server1', vnf=[Vnf{id='IDS', delay=12, deploy=30, resourceCPU=3, resourceRAM=2, resourceStorage=9, licenceCost=80.0, bandwidthFactor=0.9}, Vnf{id='Proxy', delay=5, deploy=25, resourceCPU=4, resourceRAM=3, resourceStorage=8, licenceCost=85.0, bandwidthFactor=0.5}], licenceCost=60.0, energyCost=0.1, resourceCPU=16, resourceRAM=8, resourceStorage=500, resourceCPUCost=4.0, resourceRAMCost=3.0, resourceStorageCost=2.7, energyPerCoreWatts=80, energyPeakWatts=2735, resourceRAMUsed=5, resourceStorageUsed=17, resourceCPUUsed=7, energyUsed=560}, energyCost=0.3
2020-04-25 17:39:12,011 [main           ] INFO  VnfService                     - Node:id='node3', server=Server{id='server3', vnf=[Vnf{id='Firewall', delay=4, deploy=20, resourceCPU=3, resourceRAM=4, resourceStorage=6, licenceCost=75.0, bandwidthFactor=0.8}], licenceCost=120.0, energyCost=0.25, resourceCPU=10, resourceRAM=12, resourceStorage=240, resourceCPUCost=3.0, resourceRAMCost=1.5, resourceStorageCost=3.0, energyPerCoreWatts=70, energyPeakWatts=2500, resourceRAMUsed=4, resourceStorageUsed=6, resourceCPUUsed=3, energyUsed=210}, energyCost=0.4
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Node:id='node5', server=null, energyCost=0.6
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Node:id='node6', server=null, energyCost=0.2
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Enlaces de la Solucion: 
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Link{id='node1-node4', delay=3, distance=60, bandwidth=900.0, bandwidthCost=0.2, bandwidthUsed=294.0}
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Link{id='node4-node3', delay=5, distance=55, bandwidth=500.0, bandwidthCost=0.5, bandwidthUsed=132.3}
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Link{id='node3-node5', delay=2, distance=100, bandwidth=650.0, bandwidthCost=0.5, bandwidthUsed=105.84000000000002}
2020-04-25 17:39:12,012 [main           ] INFO  VnfService                     - Link{id='node5-node6', delay=5, distance=97, bandwidth=970.0, bandwidthCost=0.2, bandwidthUsed=105.84000000000002}

2020-04-25 17:39:12,013 [main           ] INFO  VnfService                     - Funciones Objetivos con sus resultados: 
2020-04-25 17:39:12,013 [main           ] INFO  VnfService                     - Costo de Energia total: 110.7
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Costo de Reenvio de Trafico: 309.738
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Cantidad de Hosts o Servidores utilizados: 2
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Costo de latencia/Retardo/Retraso total: 36
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Costo de Instalacion o Configuracion total: 75
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Distancia total: 312
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Numero de Saltos/Numero de enlaces de la ruta: 4
2020-04-25 17:39:12,017 [main           ] INFO  VnfService                     - Ancho de banda total: 637.98
2020-04-25 17:39:12,018 [main           ] INFO  VnfService                     - Numero de instancias: 3
2020-04-25 17:39:12,020 [main           ] INFO  VnfService                     - Trafico de Carga: 22967.28
2020-04-25 17:39:12,020 [main           ] INFO  VnfService                     - Recursos total:121.9
2020-04-25 17:39:12,021 [main           ] INFO  VnfService                     - Costo por SLO: 3.0
2020-04-25 17:39:12,021 [main           ] INFO  VnfService                     - Costo de licencia total: 420.0
2020-04-25 17:39:12,021 [main           ] INFO  VnfService                     - Costo de Fragmentacion: 100.5206
2020-04-25 17:39:12,021 [main           ] INFO  VnfService                     - Costo de todos los enlaces: 199.03800000000004
2020-04-25 17:39:12,031 [main           ] INFO  VnfService                     - Maxima uitlizacion del enlace: 294.0
