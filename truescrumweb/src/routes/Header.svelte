<script>
    import { Navbar, NavBrand, NavLi, NavUl, NavHamburger } from 'flowbite-svelte'
    import { Avatar, Dropdown, DropdownItem, DropdownHeader, DropdownDivider } from 'flowbite-svelte';
    // import { ChevronDownOutline } from 'flowbite-svelte-icons';
</script>

<header>
    <Navbar color="primary">
        <NavBrand href="/">
        <img
            src="aejalin.png"
            class="mr-3 h-6 sm:h-9"
            alt="Aejalin Logo"
        />
        <span class="self-center whitespace-nowrap text-xl font-semibold dark:text-white">
            Aejalin
        </span>
        </NavBrand>
        <!-- <div class="flex items-center md:order-2">
            <Avatar id="avatar-menu" src="aejalin.png" />
            <NavHamburger class1="w-full md:flex md:w-auto md:order-1" />
        </div>
        <Dropdown placement="bottom" triggeredBy="#avatar-menu">
        <DropdownHeader>
            <span class="block text-sm">Bonnie Green</span>
            <span class="block truncate text-sm font-medium">name@flowbite.com</span>
        </DropdownHeader>
        <DropdownItem>Dashboard</DropdownItem>
        <DropdownItem>Settings</DropdownItem>
        <DropdownItem>Earnings</DropdownItem>
        <DropdownDivider />
        <DropdownItem>Sign out</DropdownItem>
        </Dropdown> -->

        <NavHamburger />

        <NavUl color="primary">
            <NavLi href="/">Home</NavLi>
            <NavLi class="cursor-pointer">Seminar</NavLi>
            <Dropdown class="w-44 z-20">
                <DropdownItem href="/seminar/agilelean">Agile & Lean</DropdownItem>
                <DropdownItem href="/seminar/okr">OKR with KPI</DropdownItem>
                <DropdownItem href="/seminar/leadership">Leadership</DropdownItem>
            </Dropdown>

            <NavLi class="cursor-pointer">Courses</NavLi>
            <Dropdown class="w-44 z-20">
                <DropdownItem href="/course/rsm">RSM</DropdownItem>
                <DropdownItem href="/course/rpo">RPO</DropdownItem>
                <DropdownItem href="/course/rsmpo">RSMPO</DropdownItem>
                <DropdownDivider />
                <DropdownItem href="/course/bdd">BDD</DropdownItem>
                <DropdownItem href="/course/tdd">TDD</DropdownItem>
                <DropdownItem href="/course/refactoring">Refacatoring</DropdownItem>
                <DropdownItem href="/course/devops">DevOps</DropdownItem>
            </Dropdown>

            <NavLi class="cursor-pointer">Consulting</NavLi>
            <Dropdown class="w-44 z-20">
                <DropdownItem href="/consulting/businessmodelcanvas">Business Model Canvas</DropdownItem>
                <DropdownItem href="/consulting/userstorymapping">User Story Mapping</DropdownItem>
                <DropdownItem href="/consulting/domainstorytelling">Domain Storytelling</DropdownItem>
                <DropdownItem href="/consulting/eventstorming">Eventstorming</DropdownItem>
                <DropdownItem href="/consulting/designthinking">Design Thinking</DropdownItem>
                <DropdownItem href="/consulting/designsprint">Design Sprint</DropdownItem>
                <DropdownDivider />
                <DropdownItem href="/consulting/enterprisebuilding">Enterprise Building</DropdownItem>
                <DropdownItem href="/consulting/teambuilding">Team Building</DropdownItem>
                <DropdownItem href="/consulting/"></DropdownItem>
            </Dropdown>

            <NavLi class="cursor-pointer">Coaching</NavLi>
            <Dropdown class="w-44 z-20">
                <DropdownItem href="/coaching/business">Business Coaching</DropdownItem>
                <DropdownItem href="/coaching/leadership">Leadership Coaching</DropdownItem>
                <DropdownDivider />
                <DropdownItem href="/coaching/enterprisescrum">Scrum Enterprise Coaching</DropdownItem>
                <DropdownItem href="/coaching/teamscrum">Scrum Team Coaching</DropdownItem>
            </Dropdown>

            <NavLi href="/contact">Contact</NavLi>
        </NavUl>
    </Navbar>
</header>
