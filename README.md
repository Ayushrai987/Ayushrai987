<!DOCTYPE html>
<!-- saved from url=(0057)file:///C:/Users/umesh/Downloads/projects_showcase_1.html -->
<html lang="en"><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
    
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ayushrai987 - Projects Showcase</title>
    <script src="./Ayushrai987 - Projects Showcase_files/chart.min.js.download"></script>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: #0A101F;
            color: #E5E7EB;
            padding: 40px 20px;
            line-height: 1.6;
        }

        .container {
            max-width: 1400px;
            margin: 0 auto;
        }

        .page-header {
            display: flex;
            align-items: center;
            gap: 16px;
            margin-bottom: 40px;
            padding-bottom: 24px;
            border-bottom: 2px solid rgba(34, 211, 238, 0.2);
        }

        .page-header h1 {
            font-size: 32px;
            font-weight: 700;
            background: linear-gradient(135deg, #A78BFA 0%, #7C3AED 100%);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .live-badge {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            background: rgba(16, 185, 129, 0.15);
            border: 1px solid #10B981;
            color: #10B981;
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 600;
        }

        .live-dot {
            width: 6px;
            height: 6px;
            background: #10B981;
            border-radius: 50%;
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0%, 100% { opacity: 1; transform: scale(1); }
            50% { opacity: 0.5; transform: scale(1.2); }
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
            gap: 24px;
            margin-bottom: 40px;
        }

        .project-card {
            background: linear-gradient(135deg, #111827 0%, #0F172A 100%);
            border: 1px solid #1E293B;
            border-radius: 16px;
            padding: 24px;
            display: flex;
            flex-direction: column;
            height: 100%;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .project-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(34, 211, 238, 0.5), transparent);
        }

        .project-card:hover {
            border-color: #22D3EE;
            box-shadow: 0 0 30px rgba(34, 211, 238, 0.15);
            transform: translateY(-6px);
        }

        .project-top {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 16px;
        }

        .project-icon-section {
            display: flex;
            align-items: center;
            gap: 12px;
            flex: 1;
        }

        .project-icon {
            width: 48px;
            height: 48px;
            border-radius: 12px;
            background: linear-gradient(135deg, #22D3EE 0%, #0891B2 100%);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            flex-shrink: 0;
        }

        .project-info {
            flex: 1;
        }

        .project-name {
            font-size: 16px;
            font-weight: 700;
            color: #F0F9FF;
            margin-bottom: 4px;
        }

        .project-description {
            font-size: 12px;
            color: #9CA3AF;
            line-height: 1.4;
        }

        .chart-container {
            width: 80px;
            height: 80px;
            position: relative;
            flex-shrink: 0;
        }

        .project-middle {
            display: flex;
            gap: 12px;
            margin-bottom: 16px;
            flex-wrap: wrap;
        }

        .tech-item {
            display: flex;
            align-items: center;
            gap: 4px;
            font-size: 11px;
            color: #9CA3AF;
        }

        .tech-dot {
            width: 6px;
            height: 6px;
            border-radius: 50%;
            flex-shrink: 0;
        }

        .tech-label {
            font-size: 11px;
            font-weight: 500;
            color: #D1D5DB;
        }

        .tech-percent {
            font-size: 11px;
            color: #6B7280;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-bottom: 16px;
        }

        .tag {
            background: rgba(167, 139, 250, 0.15);
            border: 1px solid rgba(167, 139, 250, 0.4);
            color: #A78BFA;
            padding: 4px 10px;
            border-radius: 6px;
            font-size: 11px;
            font-weight: 600;
        }

        .project-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding-top: 12px;
            border-top: 1px solid rgba(34, 211, 238, 0.1);
            margin-top: auto;
            font-size: 12px;
            color: #6B7280;
        }

        .star-count {
            display: flex;
            align-items: center;
            gap: 4px;
        }

        .updated-time {
            text-align: right;
        }

        .view-btn {
            color: #22D3EE;
            text-decoration: none;
            font-weight: 600;
            font-size: 12px;
            cursor: pointer;
            transition: color 0.3s ease;
        }

        .view-btn:hover {
            color: #10B981;
        }

        @media (max-width: 768px) {
            .projects-grid {
                grid-template-columns: 1fr;
            }

            .page-header h1 {
                font-size: 24px;
            }

            .project-top {
                flex-direction: column;
            }

            .chart-container {
                width: 60px;
                height: 60px;
            }
        }

        .legend-container {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
            margin-top: 12px;
            padding-top: 12px;
            border-top: 1px solid rgba(34, 211, 238, 0.1);
        }

        .legend-item {
            display: flex;
            align-items: center;
            gap: 6px;
            font-size: 11px;
        }

        .legend-color {
            width: 8px;
            height: 8px;
            border-radius: 50%;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header -->
        <div class="page-header">
            <h1>PROJECTS.LIST</h1>
            <span class="live-badge">
                <span class="live-dot"></span>
                6 Active Projects
            </span>
        </div>

        <!-- Projects Grid -->
        <div class="projects-grid">
            <!-- Project 1: Chronous -->
            <div class="project-card">
                <div class="project-top">
                    <div class="project-icon-section">
                        <div class="project-icon">⏱️</div>
                        <div class="project-info">
                            <div class="project-name">Chronous</div>
                            <div class="project-description">
                                Time-tracking &amp; productivity dashboard from GTBIT Hackathon
                            </div>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="chart1" width="100" height="100" style="display: block; box-sizing: border-box; height: 80px; width: 80px;"></canvas>
                    </div>
                </div>

                <div class="project-middle">
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #3B82F6;"></span>
                        <span class="tech-label">TypeScript</span>
                        <span class="tech-percent">45%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #10B981;"></span>
                        <span class="tech-label">React</span>
                        <span class="tech-percent">35%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #F59E0B;"></span>
                        <span class="tech-label">Firebase</span>
                        <span class="tech-percent">20%</span>
                    </div>
                </div>

                <div class="project-tags">
                    <span class="tag">TypeScript</span>
                    <span class="tag">React</span>
                    <span class="tag">Hackathon</span>
                </div>

                <div class="project-footer">
                    <div class="star-count">★ 1</div>
                    <div class="updated-time">updated 2d ago</div>
                </div>
            </div>

            <!-- Project 2: Carbon Footprint Platform -->
            <div class="project-card">
                <div class="project-top">
                    <div class="project-icon-section">
                        <div class="project-icon">🌍</div>
                        <div class="project-info">
                            <div class="project-name">Carbon Footprint</div>
                            <div class="project-description">
                                AI-powered environmental impact tracker with smart recommendations
                            </div>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="chart2" width="100" height="100" style="display: block; box-sizing: border-box; height: 80px; width: 80px;"></canvas>
                    </div>
                </div>

                <div class="project-middle">
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #3B82F6;"></span>
                        <span class="tech-label">TypeScript</span>
                        <span class="tech-percent">50%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #8B5CF6;"></span>
                        <span class="tech-label">AI/ML</span>
                        <span class="tech-percent">30%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #EC4899;"></span>
                        <span class="tech-label">Node.js</span>
                        <span class="tech-percent">20%</span>
                    </div>
                </div>

                <div class="project-tags">
                    <span class="tag">AI/ML</span>
                    <span class="tag">TypeScript</span>
                    <span class="tag">Web App</span>
                </div>

                <div class="project-footer">
                    <div class="star-count">★ 0</div>
                    <div class="updated-time">updated 1mo ago</div>
                </div>
            </div>

            <!-- Project 3: VoteBuddy -->
            <div class="project-card">
                <div class="project-top">
                    <div class="project-icon-section">
                        <div class="project-icon">🗳️</div>
                        <div class="project-info">
                            <div class="project-name">VoteBuddy</div>
                            <div class="project-description">
                                Secure voting application with real-time results &amp; authentication
                            </div>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="chart3" width="100" height="100" style="display: block; box-sizing: border-box; height: 80px; width: 80px;"></canvas>
                    </div>
                </div>

                <div class="project-middle">
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #3B82F6;"></span>
                        <span class="tech-label">TypeScript</span>
                        <span class="tech-percent">40%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #10B981;"></span>
                        <span class="tech-label">React</span>
                        <span class="tech-percent">35%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #06B6D4;"></span>
                        <span class="tech-label">Node.js</span>
                        <span class="tech-percent">25%</span>
                    </div>
                </div>

                <div class="project-tags">
                    <span class="tag">TypeScript</span>
                    <span class="tag">React</span>
                    <span class="tag">Secure</span>
                </div>

                <div class="project-footer">
                    <div class="star-count">★ 0</div>
                    <div class="updated-time">updated 3mo ago</div>
                </div>
            </div>

            <!-- Project 4: Terrai AI -->
            <div class="project-card">
                <div class="project-top">
                    <div class="project-icon-section">
                        <div class="project-icon">🤖</div>
                        <div class="project-info">
                            <div class="project-name">Terrai AI</div>
                            <div class="project-description">
                                Machine learning project for terrain analysis and predictive modeling
                            </div>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="chart4" width="100" height="100" style="display: block; box-sizing: border-box; height: 80px; width: 80px;"></canvas>
                    </div>
                </div>

                <div class="project-middle">
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #F59E0B;"></span>
                        <span class="tech-label">Python</span>
                        <span class="tech-percent">60%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #8B5CF6;"></span>
                        <span class="tech-label">ML/AI</span>
                        <span class="tech-percent">28%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #EF4444;"></span>
                        <span class="tech-label">NumPy</span>
                        <span class="tech-percent">12%</span>
                    </div>
                </div>

                <div class="project-tags">
                    <span class="tag">Python</span>
                    <span class="tag">ML/AI</span>
                    <span class="tag">NumPy</span>
                </div>

                <div class="project-footer">
                    <div class="star-count">★ 0</div>
                    <div class="updated-time">updated 5mo ago</div>
                </div>
            </div>

            <!-- Project 5: Creative Codex -->
            <div class="project-card">
                <div class="project-top">
                    <div class="project-icon-section">
                        <div class="project-icon">📚</div>
                        <div class="project-info">
                            <div class="project-name">Creative Codex</div>
                            <div class="project-description">
                                Xenothon competition project with creative coding solutions
                            </div>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="chart5" width="100" height="100" style="display: block; box-sizing: border-box; height: 80px; width: 80px;"></canvas>
                    </div>
                </div>

                <div class="project-middle">
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #F59E0B;"></span>
                        <span class="tech-label">Python</span>
                        <span class="tech-percent">55%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #06B6D4;"></span>
                        <span class="tech-label">Jupyter</span>
                        <span class="tech-percent">30%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #EC4899;"></span>
                        <span class="tech-label">DSA</span>
                        <span class="tech-percent">15%</span>
                    </div>
                </div>

                <div class="project-tags">
                    <span class="tag">Python</span>
                    <span class="tag">Jupyter</span>
                    <span class="tag">Competition</span>
                </div>

                <div class="project-footer">
                    <div class="star-count">★ 0</div>
                    <div class="updated-time">updated 4mo ago</div>
                </div>
            </div>

            <!-- Project 6: LeetCode Solutions -->
            <div class="project-card">
                <div class="project-top">
                    <div class="project-icon-section">
                        <div class="project-icon">💻</div>
                        <div class="project-info">
                            <div class="project-name">LeetCode Solutions</div>
                            <div class="project-description">
                                Optimized DSA solutions with detailed explanations &amp; edge cases
                            </div>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="chart6" width="100" height="100" style="display: block; box-sizing: border-box; height: 80px; width: 80px;"></canvas>
                    </div>
                </div>

                <div class="project-middle">
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #EF4444;"></span>
                        <span class="tech-label">Java</span>
                        <span class="tech-percent">50%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #F59E0B;"></span>
                        <span class="tech-label">Python</span>
                        <span class="tech-percent">35%</span>
                    </div>
                    <div class="tech-item">
                        <span class="tech-dot" style="background: #10B981;"></span>
                        <span class="tech-label">C++</span>
                        <span class="tech-percent">15%</span>
                    </div>
                </div>

                <div class="project-tags">
                    <span class="tag">Java</span>
                    <span class="tag">Python</span>
                    <span class="tag">Algorithms</span>
                </div>

                <div class="project-footer">
                    <div class="star-count">★ 0</div>
                    <div class="updated-time">updated 1w ago</div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Chart.js configuration with gradient colors
        const chartConfig = {
            responsive: true,
            maintainAspectRatio: false,
            plugins: {
                legend: {
                    display: false
                }
            }
        };

        // Chart 1: Chronous
        const ctx1 = document.getElementById('chart1').getContext('2d');
        new Chart(ctx1, {
            type: 'doughnut',
            data: {
                labels: ['TypeScript', 'React', 'Firebase'],
                datasets: [{
                    data: [45, 35, 20],
                    backgroundColor: [
                        '#3B82F6',
                        '#10B981',
                        '#F59E0B'
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 2
                }]
            },
            options: chartConfig
        });

        // Chart 2: Carbon Footprint
        const ctx2 = document.getElementById('chart2').getContext('2d');
        new Chart(ctx2, {
            type: 'doughnut',
            data: {
                labels: ['TypeScript', 'AI/ML', 'Node.js'],
                datasets: [{
                    data: [50, 30, 20],
                    backgroundColor: [
                        '#3B82F6',
                        '#8B5CF6',
                        '#EC4899'
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 2
                }]
            },
            options: chartConfig
        });

        // Chart 3: VoteBuddy
        const ctx3 = document.getElementById('chart3').getContext('2d');
        new Chart(ctx3, {
            type: 'doughnut',
            data: {
                labels: ['TypeScript', 'React', 'Node.js'],
                datasets: [{
                    data: [40, 35, 25],
                    backgroundColor: [
                        '#3B82F6',
                        '#10B981',
                        '#06B6D4'
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 2
                }]
            },
            options: chartConfig
        });

        // Chart 4: Terrai AI
        const ctx4 = document.getElementById('chart4').getContext('2d');
        new Chart(ctx4, {
            type: 'doughnut',
            data: {
                labels: ['Python', 'ML/AI', 'NumPy'],
                datasets: [{
                    data: [60, 28, 12],
                    backgroundColor: [
                        '#F59E0B',
                        '#8B5CF6',
                        '#EF4444'
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 2
                }]
            },
            options: chartConfig
        });

        // Chart 5: Creative Codex
        const ctx5 = document.getElementById('chart5').getContext('2d');
        new Chart(ctx5, {
            type: 'doughnut',
            data: {
                labels: ['Python', 'Jupyter', 'DSA'],
                datasets: [{
                    data: [55, 30, 15],
                    backgroundColor: [
                        '#F59E0B',
                        '#06B6D4',
                        '#EC4899'
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 2
                }]
            },
            options: chartConfig
        });

        // Chart 6: LeetCode Solutions
        const ctx6 = document.getElementById('chart6').getContext('2d');
        new Chart(ctx6, {
            type: 'doughnut',
            data: {
                labels: ['Java', 'Python', 'C++'],
                datasets: [{
                    data: [50, 35, 15],
                    backgroundColor: [
                        '#EF4444',
                        '#F59E0B',
                        '#10B981'
                    ],
                    borderColor: '#0F172A',
                    borderWidth: 2
                }]
            },
            options: chartConfig
        });
    </script>


</body></html>
