<template>
    <div class="shadow">
                <!-- Topbar -->
                <nav class="navbar navbar-expand navbar-light bg-white topbar static-top" id="top">
                    <div class="container">
                        <!-- toggle navigasi  (Visible Only XS) -->
                        <ul class="navbar-nav">
                        <li class="nav-item dropdown no-arrow d-sm-none">
                            <button class="btn btn-link d-md-none rounded-circle mr-3" id="sidebarToggleTop" role="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                            <i class="fa fa-bars"></i>
                            </button>
                        </li>
                        </ul>
                        
                        <h3 style="color:black; font-family: 'Lato', sans-serif;">JURNAL UANG</h3>
                        
                        <!-- Topbar Navbar -->
                        <ul class="navbar-nav ml-auto">
                            <li class="nav-item dropdown my-auto mx-2" id="search">
                                <!-- Topbar Search -->
                                <div class="input-group">
                                  <input class="form-control bg-light border-0 small" placeholder="Search for..." name="search" type="text">
                                    <div class="input-group-append">
                                        <div class="btn-group">
                                            <select class="btn btn-secondary dropdown-toggle" name="filter"><option value="reimbursement">Reimbursements</option><option value="bill">Bills</option><option value="report">Reports</option></select>
                                            <button type="submit" class="btn btn-primary"><i class="fas fa-search fa-sm"></i></button>
                                    </div>
                                </div>
                                </div>
                            </li>
                        <!-- Nav Item - Search Dropdown (Visible Only XS) -->
                        <li class="nav-item dropdown no-arrow d-sm-none">
                            <a class="nav-link dropdown-toggle" href="#" id="searchDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            <i class="fas fa-search fa-fw"></i>
                            </a>
                            <!-- Dropdown - Messages -->
                            <div class="dropdown-menu dropdown-menu-right p-3 shadow animated--grow-in" aria-labelledby="searchDropdown">
                            <form class="form-inline mr-auto w-100 navbar-search">
                                <div class="input-group">
                                <input type="text" class="form-control bg-light border-0 small" placeholder="Search for..." aria-label="Search" aria-describedby="basic-addon2">
                                <div class="input-group-append">
                                    <button class="btn btn-primary" type="button">
                                    <i class="fas fa-search fa-sm"></i>
                                    </button>
                                </div>
                                </div>
                            </form>
                            </div>
                        </li>

                        <!-- Nav Item - Alerts -->
                        <li class="nav-item dropdown no-arrow mx-1">
                            <a class="nav-link dropdown-toggle" href="#" id="alertsDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            <i class="fas fa-bell fa-fw"></i>
                            <!-- Counter - Alerts -->
                            <span class="badge badge-danger badge-counter"></span>
                            </a>
                            <!-- Dropdown - Alerts -->
                            <div class="dropdown-list dropdown-menu dropdown-menu-right shadow animated--grow-in" aria-labelledby="alertsDropdown">
                                <h6 class="dropdown-header">
                                    Nofification
                                </h6>
                                <a class="dropdown-item d-flex align-items-center" href="#" data-toggle="modal" data-target="">
                                
                                    <div class="mr-3">
                                        <div class="icon-circle bg-warning">
                                            <i class="fas fa-exchange-alt text-white"></i>
                                        </div>
                                        <div class="icon-circle bg-danger">
                                            <i class="fas fa-file-alt text-white"></i>
                                        </div>
                                        
                                    </div>
                                    <div>
                                        <div class="small text-gray-500"></div>
                                        <p class="font-weight-bold"></p>
                                        <small></small>
                                    </div>
                                </a>
                            </div>
                        </li>
                        <!-- Nav Item - User Information -->
                        <li class="nav-item dropdown no-arrow">
                            <a class="nav-link dropdown-toggle" href="#" id="userDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                            <img class="img-profile rounded-circle" src="https://source.unsplash.com/QAB-WJcbgJk/60x60">
                            </a>
                            <!-- Dropdown - User Information -->
                            <div class="dropdown-menu dropdown-menu-right shadow animated--grow-in" aria-labelledby="userDropdown">
                            <a class="dropdown-item" href="/profile">
                                <i class="fas fa-user fa-sm fa-fw mr-2 text-gray-400"></i>
                                Profile
                            </a>
                            @role('admin')
                                <a class="dropdown-item" href="/users">
                                    <i class="fa fa-users mr-2 text-gray-400"></i>
                                    User Management
                                </a>
                            @endrole
                            @role('member')
                                <a class="dropdown-item" href="/banks">
                                    <i class="far fa-credit-card mr-2 text-gray-400"></i>
                                    Bank Accounts Management
                                </a>
                            @endrole
                            <a class="dropdown-item" href="/log">
                            <i class="fa fa-history fa-sm fa-fw mr-2 text-gray-400"></i>
                                Activity Log
                            </a>
                            <div class="dropdown-divider"></div>
                            <a class="dropdown-item" href="#" data-toggle="modal" data-target="#logoutModal">
                                <i class="fas fa-sign-out-alt fa-sm fa-fw mr-2 text-gray-400"></i>
                                Logout
                            </a>
                            </div>
                        </li>
                        </ul>
                    </div>
                </nav>
                <!-- navigasi -->
                <nav class="navbar navbar-expand-sm navbar-light bg-white border-top" style="font-size:16px;">
                    <div class="container">
                        <div class="collapse navbar-collapse " id="navbarNav">
                            <ul class="navbar-nav">
                            <li class="nav-item ">
                                <a class="nav-link" href="/">Dashboard</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="/daily_reports">Cash Reports</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="/reimbursements">Reimbursements</a>
                            </li>
                            <li class="nav-item">
                                <a class="nav-link" href="/bills">Bills</a>
                            </li> 
                            </ul>
                        </div>
                    </div>
                </nav>
            </div>
</template>