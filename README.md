<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=0,99,153,102,51&height=280&section=header&text=Moeez%20Ahmed%20Dar&fontSize=80&fontAlignY=45&animation=twinkling&fontColor=ffffff" width="100%" alt="Header" />
  <h2 style="margin-top:-30px; color:#6366f1; font-family:'Fira Code', monospace;">Full Stack Software Engineer</h2>
</div>

<div align="center">
  <a href="https://www.linkedin.com/in/moeez-ahmed-b39664185/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="mailto:moeezahmed448@gmail.com" target="_blank">
    <img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="tel:+447555859884" target="_blank">
    <img src="https://img.shields.io/badge/Phone-+44%207555%20859884-25D366?style=for-the-badge&logo=whatsapp&logoColor=white" alt="Phone" />
  </a>
  <img src="https://komarev.com/ghpvc/?username=MoeezAhmedDar&color=00C4B4&style=for-the-badge&label=Profile+Views" alt="Profile Views" />
</div>

<br />

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=36&pause=1200&color=00C4B4&center=true&vCenter=true&width=800&lines=Full+Stack+Software+Engineer;Laravel+%26+PHP+Specialist;Passionate+about+Scalable+Systems" alt="Typing SVG" />
</div>

<br />

<h2 align="center">About Me</h2>

<p align="center">
  I'm a dedicated developer with over three years of experience creating reliable web applications using Laravel and PHP.  
  I enjoy solving real business problems through efficient, well-organized code — from automating workflows to building real-time features and powerful reporting tools.  
  Recently completed my Master's in Artificial Intelligence, which has deepened my interest in adding intelligent capabilities to software.
</p>

<br />

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=MoeezAhmedDar&show_icons=true&theme=radical&hide_border=true&include_all_commits=true&count_private=true" alt="Moeez's GitHub Stats" width="48%" />
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=MoeezAhmedDar&theme=radical&hide_border=true" alt="GitHub Streak" width="48%" />
</div>

<br />

<h2 align="center">Skills & Technologies</h2>

<div align="center">
  <img src="https://skillicons.dev/icons?i=laravel,php,javascript,jquery,mysql,mongodb,aws,docker,git,github" alt="Skills Icons" width="70%" />
</div>

<br />

<h2 align="center">A Little Laravel Example</h2>

<p align="center">
  Here's a clean, modern Laravel job example (queueable + notification) — one of the things I enjoy building!
</p>

```php
<?php

namespace App\Jobs;

use Illuminate\Bus\Queueable;
use Illuminate\Contracts\Queue\ShouldQueue;
use Illuminate\Foundation\Bus\Dispatchable;
use Illuminate\Queue\InteractsWithQueue;
use Illuminate\Queue\SerializesModels;
use Illuminate\Support\Facades\Log;
use App\Notifications\ReportGenerated;

class GenerateDailyReport implements ShouldQueue
{
    use Dispatchable, InteractsWithQueue, Queueable, SerializesModels;

    protected $user;

    public function __construct($user)
    {
        $this->user = $user;
    }

    public function handle(): void
    {
        try {
            // Simulate heavy report generation (e.g., query large data, PDF creation)
            sleep(5); // In real life: Excel/PDF generation, complex DB queries

            // Send success notification
            $this->user->notify(new ReportGenerated('Daily report generated successfully!'));

            Log::info('Daily report generated for user: ' . $this->user->email);
        } catch (\Exception $e) {
            // Log error & retry (Laravel handles retries automatically)
            Log::error('Report generation failed: ' . $e->getMessage());
            $this->fail($e);
        }
    }
}

Dispatch it like this: GenerateDailyReport::dispatch($user)->delay(now()->addMinutes(5));



Education

  Master of Science in Artificial Intelligence

  University of Stirling, Stirling, Scotland (Completed September 2025)


  Bachelor of Science in Computer Science

  BUITEMS, Quetta, Pakistan (2017 – 2021)



Let's Connect

  
    LinkedIn
  
  
    Email
  
  
    Phone
  




  Building reliable software with passion and precision. 🚀


  Footer
