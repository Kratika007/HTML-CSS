# HTML-CSS

<!DOCTYPE html>
<html lang="en">

<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>System Monitoring Dashboard</title>

    <!-- Google Font -->

    <link rel="preconnect" href="https://fonts.googleapis.com">

    <link
        href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap"
        rel="stylesheet">

    <!-- Font Awesome -->

    <link rel="stylesheet"
        href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

  <style>

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Poppins',sans-serif;
}

body{
    background:#0f172a;
    color:white;
}

/* Sidebar */
.sidebar{
    width:260px;
    height:100vh;
    position:fixed;
    left:0;
    top:0;
    background:linear-gradient(to bottom,#111827,#1e293b);
    padding:25px;
}

.logo{
    font-size:28px;
    font-weight:700;
    color:#60a5fa;
    margin-bottom:40px;
}

.logo span{
    color:#c084fc;
}

.menu{
    list-style:none;
    padding-left:0;
}

.menu li{
    margin:15px 0;
}

.menu a{
    text-decoration:none;
    color:#cbd5e1;
    padding:12px;
    display:block;
    border-radius:10px;
}

.menu a:hover{
    background:#3b82f6;
    color:white;
}

/* Main */
.main{
    margin-left:260px;
    padding:30px;
}

/* Topbar */
.topbar{
    display:flex;
    justify-content:space-between;
    align-items:center;
    margin-bottom:30px;
}

.profile{
    display:flex;
    align-items:center;
    gap:15px;
}

.profile img{
    width:50px;
    height:50px;
    border-radius:50%;
}

/* Cards */
.stat-card{
    background:#1e293b;
    border-radius:20px;
    padding:25px;
    height:100%;
}

.icon-box{
    width:60px;
    height:60px;
    border-radius:15px;
    display:flex;
    align-items:center;
    justify-content:center;
    font-size:24px;
    margin-bottom:15px;
}

.bg-blue{background:#2563eb;}
.bg-purple{background:#7c3aed;}
.bg-green{background:#059669;}
.bg-orange{background:#ea580c;}

.card-value{
    font-size:30px;
    font-weight:700;
}

/* Sections */
.monitor-card,
.table-card,
.chart-box,
.logs-card{
    background:#1e293b;
    padding:25px;
    border-radius:20px;
    margin-top:30px;
}

/* Progress */
.progress{
    height:20px;
    margin-top:8px;
}

/* Status */
.status{
    padding:6px 12px;
    border-radius:20px;
    font-size:12px;
}

.online{
    background:green;
}

.warning{
    background:orange;
}

.offline{
    background:red;
}

/* Chart */
.fake-chart{
    display:flex;
    align-items:flex-end;
    justify-content:space-between;
    height:220px;
    margin-top:20px;
}

.bar{
    width:35px;
    background:linear-gradient(to top,#3b82f6,#8b5cf6);
    border-radius:10px 10px 0 0;
}

/* Logs */
.logs-card textarea{
    width:100%;
    height:250px;
    background:#0f172a;
    color:#22c55e;
    border:none;
    padding:15px;
    border-radius:15px;
}

/* Responsive */
@media(max-width:992px){

    .sidebar{
        width:100%;
        height:auto;
        position:relative;
    }

    .main{
        margin-left:0;
    }

}

</style>

</head>

<body>

    <!-- Sidebar -->

    <div class="sidebar">

        <div class="logo">
            System<span>Panel</span>
        </div>

        <ul class="menu">

            <li>
                <a href="#Dashboard">
                    <i class="fa-solid fa-chart-line"></i>
                    Dashboard
                </a>
            </li>

            <li>
                <a href="#Servers">
                    <i class="fa-solid fa-server"></i>
                    Servers
                </a>
            </li>

            <li>
                <a href="#Database">
                    <i class="fa-solid fa-database"></i>
                    Database
                </a>
            </li>

            <li>
                <a href="#Network">
                    <i class="fa-solid fa-network-wired"></i>
                    Network
                </a>
            </li>

            <li>
                <a href="#Security">
                    <i class="fa-solid fa-user-shield"></i>
                    Security
                </a>
            </li>

            <li>
                <a href="#Settings">
                    <i class="fa-solid fa-gear"></i>
                    Settings
                </a>
            </li>

            <li>
                <a href="#Logout">
                    <i class="fa-solid fa-right-from-bracket"></i>
                    Logout
                </a>
            </li>

        </ul>

    </div>

    <!-- Main Content -->

    <div class="main">

        <!-- Topbar -->

        <div class="topbar">

            <div>

                <h1>System Monitoring Dashboard</h1>

                <p>Track your server performance and system health</p>



                    <h6>Admin User</h6>

                    <small class="text-secondary">
                        System Administrator
                    </small>

                </div>

               </div><a href="#">
<i class="fa-solid fa-circle-user"></i></a>
Profile

                <div>

            </div>

        </div>

        <!-- Cards -->

        <div class="row g-4">

            <div class="col-lg-3 col-md-6">

                <div class="stat-card">

                    <div class="icon-box bg-blue">
                        <i class="fa-solid fa-microchip"></i>
                    </div>

                    <div class="card-title">
                        CPU Usage
                    </div>

                    <div class="card-value">
                        72%
                    </div>

                    <div class="small-text">
                        Running smoothly
                    </div>

                </div>

            </div>

            <div class="col-lg-3 col-md-6">

                <div class="stat-card">

                    <div class="icon-box bg-purple">
                        <i class="fa-solid fa-memory"></i>
                    </div>

                    <div class="card-title">
                        RAM Usage
                    </div>

                    <div class="card-value">
                        65%
                    </div>

                    <div class="small-text">
                        Stable memory status
                    </div>

                </div>

            </div>

            <div class="col-lg-3 col-md-6">

                <div class="stat-card">

                    <div class="icon-box bg-green">
                        <i class="fa-solid fa-hard-drive"></i>
                    </div>

                    <div class="card-title">
                        Storage
                    </div>

                    <div class="card-value">
                        81%
                    </div>

                    <div class="small-text">
                        Disk nearly full
                    </div>

                </div>

            </div>

            <div class="col-lg-3 col-md-6">

                <div class="stat-card">

                    <div class="icon-box bg-orange">
                        <i class="fa-solid fa-wifi"></i>
                    </div>

                    <div class="card-title">
                        Network Speed
                    </div>

                    <div class="card-value">
                        920Mb/s
                    </div>

                    <div class="small-text">
                        Excellent connectivity
                    </div>

                </div>

            </div>

        </div>

        <!-- Progress Section -->

        <div class="monitor-card">

            <div class="monitor-title">

                <h3>Server Performance</h3>

                <span class="badge bg-primary">
                    Live Monitoring
                </span>

            </div>

            <div class="mb-4">

                <div class="d-flex justify-content-between mb-2">

                    <span>CPU Performance</span>

                    <span>72%</span>

                </div>

                <div class="progress">

                    <div class="progress-bar bg-primary" style="width:72%">
                        72%
                    </div>

                </div>

            </div>

            <div class="mb-4">

                <div class="d-flex justify-content-between mb-2">

                    <span>RAM Consumption</span>

                    <span>65%</span>

                </div>

                <div class="progress">

                    <div class="progress-bar bg-success" style="width:65%">
                        65%
                    </div>

                </div>

            </div>

            <div class="mb-4">

                <div class="d-flex justify-content-between mb-2">

                    <span>Storage Capacity</span>

                    <span>81%</span>

                </div>

                <div class="progress">

                    <div class="progress-bar bg-warning" style="width:81%">
                        81%
                    </div>

                </div>

            </div>

        </div>

        <!-- Logs -->

        <div class="logs-card">

            <div class="monitor-title">

                <h3>System Logs</h3>

            </div>

<textarea readonly>

[10:02:15] Server started successfully...
[10:04:18] Database connection established...
[10:05:01] Security firewall activated...
[10:07:23] User admin logged in...
[10:10:40] Backup process initialized...
[10:13:11] RAM usage reached 65%...
[10:15:55] CPU temperature normal...
[10:18:32] Network latency optimized...
[10:22:09] Security scan completed...

</textarea>

        </div>

    </div>

</body>
</html>
